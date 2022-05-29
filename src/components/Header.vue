<template>
  <div class="welcome_screen">
    <div class="title">
      <h1 class="first_title">Lorem</h1>
      <h1 class="second_title">Ipsum</h1>
    </div>
    <div class="paragraph">
      <p>
        Lorem Ipsum is simply dummy text of the printing and typesetting
        industry. Lorem Ipsum has been the industry's standard dummy text ever
        since the 1500s, when an unknown printer took a galley of type and
        scrambled it to make a type specimen book. It has survived not only five
        centuries, but also the leap into electronic typesetting, remaining
        essentially unchanged.
      </p>
      <br />
      <br />
      <p>
        It was popularised in the 1960s with the release of Letraset sheets
        containing Lorem Ipsum passages, and more recently with desktop
        publishing software like Aldus PageMaker including versions of Lorem
        Ipsum.
      </p>
    </div>
    <div class="footer">
      <!-- An emit is set on the click event - this will trigger in the parent (app.vue) -->
      <button @click="$emit('startQuiz')" class="start_btn">Start Quiz</button>
    </div>
  </div>
</template>
<style>
.title {
  display: flex;
  position: absolute;
  top: 50px;
  left: 50%;
  transform: translateX(-50%);
}
.first_title {
  font-family: 'Nunito';
  font-style: normal;
  font-size: 36px;
  line-height: 120%;
  font-weight: 400;
}
.second_title {
  font-family: 'Nunito';
  font-style: normal;
  font-size: 36px;
  line-height: 120%;
  font-weight: 700;
}
.paragraph {
  position: relative;
  left: 50%;
  transform: translateX(-50%);
  top: 150px;
}
.paragraph p {
  font-family: 'Nunito';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 160%;
  padding: 0 59px;
}
.footer {
  position: absolute;
  bottom: 0;
  background-color: #000000;
  box-shadow: 0px -5px 50px rgba(15, 26, 66, 0.05);
  border-radius: 20px;
  width: 100%;
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}
.start_btn {
  background: #ffffff;
  border-radius: 10px;
  width: 178px;
  height: 40px;
  font-family: 'Rubik';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;
  letter-spacing: -0.3px;
  border: none;
  cursor: pointer;
}
</style>
