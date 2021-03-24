<template>
  <div class="meme">
    <img class="meme-img" :src="'/meme/' + image" />
    <h3 class="meme-desc">Erreicht: {{ text }}</h3>
    <div class="meme-comment-section">
      <div ref="comments" class="hidden">
        <div class="comment-close" @click="onClose()">
          <img class="icon" src="/img/up-arrow.svg" />
          Schließen
          <img class="icon" src="/img/up-arrow.svg" />
        </div>
        <div v-for="comment in comments" :key="comment.text" class="comment">
          <img :src="comment.img" /> {{ comment.name }}: {{ comment.text }}
        </div>
        <span ref="deleted" class="delete-msg hidden"
          >Hario Mofer hat deinen Kommentar gelöscht. Begründung: "Deine Meinung
          ist uns den Serverspeicher nicht wert."
        </span>
      </div>

      <div class="comment-input">
        <input placeholder="Deine Meinung..." @focus="onFocus()" />
        <button :disabled="isDisabled()" @click.prevent="sendCommant()">
          Kommentieren
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import {
  commentEntries,
  hmCommentEntries,
} from "../static/comments/comments.js";

export default {
  props: {
    image: {
      type: String,
    },
    text: {
      type: String,
      default() {
        return "sinnvolle Vertreterarbeit!";
      },
    },
  },
  created: function () {
    this.comments.push(
      hmCommentEntries[Math.floor(Math.random() * hmCommentEntries.length)]
    );

    const cmts = 2 + Math.floor(Math.random() * 3);
    let prevIndexes = [];
    for (let i = 0; i < cmts; i++) {
      let index;
      do {
        index = Math.floor(Math.random() * commentEntries.length);
      } while (prevIndexes.includes(index));

      prevIndexes.push(index);
      this.comments.push(commentEntries[index]);
    }
  },
  methods: {
    onFocus() {
      this.$refs.comments.classList.remove("hidden");
      this.disabled = false;
    },
    onClose() {
      this.$refs.comments.classList.add("hidden");
    },
    sendCommant() {
      this.$refs.comments.classList.remove("hidden");
      this.$refs.deleted.classList.remove("hidden");
    },
    isDisabled() {
      return this.disabled;
    },
  },
  data: function () {
    return {
      disabled: true,
      comments: [],
    };
  },
};
</script>

<style>
.meme {
  width: 100%;
  border: 1px solid;
  text-align: center;
  margin-bottom: 20px;
}

.meme-img {
  max-width: 100%;
  max-height: 700px;
  padding-bottom: 15px;
}

.meme-comment-section {
  width: 100%;
  border-top: 1px solid;
}

.meme-comment-section .comment {
  width: 100%;
  text-align: left;
  padding: 0 15px;
  margin: 5px 0;
}

.meme-comment-section .comment img {
  width: 50px;
  height: 50px;
}

.meme-comment-section .comment-close {
  width: 100%;
  height: 20px;
  font-size: 15px;
}

.meme-comment-section .comment-close:hover {
  background: #ededed;
}

.meme-comment-section .comment-close img {
  width: 10px;
  height: 10px;
}

.meme-comment-section input {
  width: 72%;
}

.meme-comment-section button {
  width: 26%;
}

.meme-comment-section .hidden {
  visibility: hidden;
  display: none;
}

.meme-comment-section .delete-msg {
  color: red;
  font-size: 12px;
}

.meme-comment-section .comment-input {
  margin: 5px 0;
}
</style>
