<template>
  <button>
    <span class="box"> 唔要 </span>
  </button>
</template>

<style scoped>
button {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 5px;
  background: #4b4b4b;
  font-family: "Montserrat", sans-serif;
  overflow: hidden;
  border: 1px solid #4b4b4b;
  cursor: pointer;
}

button:after {
  content: " ";
  width: 0%;
  height: 100%;
  background: #fff;
  position: absolute;
  transition: all 0.4s ease-in-out;
  right: 0;
}

button:hover::after {
  right: auto;
  left: 0;
  width: 100%;
}

button span {
  text-align: center;
  text-decoration: none;
  width: 100%;
  padding: 18px 25px;
  color: #fffcfd;
  font-size: 1.125em;
  font-weight: 700;
  letter-spacing: 0.3em;
  z-index: 20;
  transition: all 0.3s ease-in-out;
}

button:hover span {
  animation: scaleUp 0.3s ease-in-out;
  color: #4b4b4b;
}

button:hover {
  animation: scaleUp 0.3s ease-in-out;
}

</style>
