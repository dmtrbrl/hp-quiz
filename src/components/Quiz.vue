<template>
  <section class="quiz">
    <div class="welcome">
      <Picture
        class="quiz-img"
        url="https://media0.giphy.com/media/Bh3YfliwBZNwk/giphy.gif?cid=3640f6095c852266776c6f746fb2fc67"
      />
      <h1 class="quiz-heading">How Well Do You Know
        <br>the Harry Potter Movies?
      </h1>
      <a href="#" class="quiz-button">Start Quiz</a>
    </div>
  </section>
</template>

<script>
import Picture from "./Picture";
export default {
  name: "Quiz",
  components: { Picture }
};
</script>

<style>
.quiz {
  max-width: 520px;
}

.quiz-img {
  display: block;
  width: 100%;
  height: auto;
}

.quiz-heading {
  margin: 30px 0;
  font-size: 22px;
  line-height: 1.2;
}
@media (min-width: 520px) {
  .quiz-heading {
    font-size: 30px;
  }
}

.quiz-button {
  display: inline-block;
  padding: 10px 30px;
  border: 1px solid #999;
  color: #999;
  text-decoration: none;
  transition: background 0.5s, color 0.5s;
}
.quiz-button:hover {
  background: #999999;
  color: #000000;
}
</style>
