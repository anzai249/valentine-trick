<template>
  <button>
    <span class="box"> YES </span>
    <div class="star-1">
      <svg
        height="25"
        width="25"
        viewBox="0 0 512 512"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M427.313,88.686c-47.803-47.803-125.213-47.803-173.016,0l-17.087,17.087l-17.087-17.087
    c-47.803-47.803-125.213-47.803-173.016,0c-47.803,47.803-47.803,125.213,0,173.016l190.103,190.103
    c4.88,4.88,11.316,7.322,17.752,7.322c6.435,0,13.871-2.442,18.751-7.322l190.103-190.103
    C475.116,213.899,475.116,136.489,427.313,88.686z"
          fill="#fd1853"
        ></path>
      </svg>
    </div>
    <div class="star-2">
      <svg
        height="20"
        width="20"
        viewBox="0 0 512 512"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M427.313,88.686c-47.803-47.803-125.213-47.803-173.016,0l-17.087,17.087l-17.087-17.087
    c-47.803-47.803-125.213-47.803-173.016,0c-47.803,47.803-47.803,125.213,0,173.016l190.103,190.103
    c4.88,4.88,11.316,7.322,17.752,7.322c6.435,0,13.871-2.442,18.751-7.322l190.103-190.103
    C475.116,213.899,475.116,136.489,427.313,88.686z"
          fill="#fd1853"
        ></path>
      </svg>
    </div>
    <div class="star-3">
      <svg
        height="9"
        width="9"
        viewBox="0 0 512 512"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M427.313,88.686c-47.803-47.803-125.213-47.803-173.016,0l-17.087,17.087l-17.087-17.087
    c-47.803-47.803-125.213-47.803-173.016,0c-47.803,47.803-47.803,125.213,0,173.016l190.103,190.103
    c4.88,4.88,11.316,7.322,17.752,7.322c6.435,0,13.871-2.442,18.751-7.322l190.103-190.103
    C475.116,213.899,475.116,136.489,427.313,88.686z"
          fill="#fd1853"
        ></path>
      </svg>
    </div>
    <div class="star-4">
      <svg
        height="10"
        width="10"
        viewBox="0 0 512 512"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M427.313,88.686c-47.803-47.803-125.213-47.803-173.016,0l-17.087,17.087l-17.087-17.087
    c-47.803-47.803-125.213-47.803-173.016,0c-47.803,47.803-47.803,125.213,0,173.016l190.103,190.103
    c4.88,4.88,11.316,7.322,17.752,7.322c6.435,0,13.871-2.442,18.751-7.322l190.103-190.103
    C475.116,213.899,475.116,136.489,427.313,88.686z"
          fill="#fd1853"
        ></path>
      </svg>
    </div>
    <div class="star-5">
      <svg
        height="20"
        width="20"
        viewBox="0 0 512 512"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M427.313,88.686c-47.803-47.803-125.213-47.803-173.016,0l-17.087,17.087l-17.087-17.087
    c-47.803-47.803-125.213-47.803-173.016,0c-47.803,47.803-47.803,125.213,0,173.016l190.103,190.103
    c4.88,4.88,11.316,7.322,17.752,7.322c6.435,0,13.871-2.442,18.751-7.322l190.103-190.103
    C475.116,213.899,475.116,136.489,427.313,88.686z"
          fill="#fd1853"
        ></path>
      </svg>
    </div>
    <div class="star-6">
      <svg
        height="7"
        width="7"
        viewBox="0 0 512 512"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M427.313,88.686c-47.803-47.803-125.213-47.803-173.016,0l-17.087,17.087l-17.087-17.087
    c-47.803-47.803-125.213-47.803-173.016,0c-47.803,47.803-47.803,125.213,0,173.016l190.103,190.103
    c4.88,4.88,11.316,7.322,17.752,7.322c6.435,0,13.871-2.442,18.751-7.322l190.103-190.103
    C475.116,213.899,475.116,136.489,427.313,88.686z"
          fill="#fd1853"
        ></path>
      </svg>
    </div>
  </button>
</template>

<style scoped>
button {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 5px;
  background: #fd1853;
  font-family: "Montserrat", sans-serif;
  overflow: hidden;
  border: 1px solid #fd1853;
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
  color: #fd1853;
}

button:hover {
  animation: scaleUp 0.3s ease-in-out;
}

.star-1 {
  position: absolute;
  top: 20%;
  left: 20%;
  width: 25px;
  height: auto;
  filter: drop-shadow(0 0 0 #fd1853);
  z-index: -5;
  transition: all 1s cubic-bezier(0.05, 0.83, 0.43, 0.96);
}

.star-2 {
  position: absolute;
  top: 45%;
  left: 45%;
  width: 15px;
  height: auto;
  filter: drop-shadow(0 0 0 #fd1853);
  z-index: -5;
  transition: all 1s cubic-bezier(0, 0.4, 0, 1.01);
}

.star-3 {
  position: absolute;
  top: 40%;
  left: 40%;
  width: 5px;
  height: auto;
  filter: drop-shadow(0 0 0 #fd1853);
  z-index: -5;
  transition: all 1s cubic-bezier(0, 0.4, 0, 1.01);
}

.star-4 {
  position: absolute;
  top: 20%;
  left: 40%;
  width: 8px;
  height: auto;
  filter: drop-shadow(0 0 0 #fd1853);
  z-index: -5;
  transition: all 0.8s cubic-bezier(0, 0.4, 0, 1.01);
}

.star-5 {
  position: absolute;
  top: 25%;
  left: 45%;
  width: 15px;
  height: auto;
  filter: drop-shadow(0 0 0 #fd1853);
  z-index: -5;
  transition: all 0.6s cubic-bezier(0, 0.4, 0, 1.01);
}

.star-6 {
  position: absolute;
  top: 5%;
  left: 50%;
  width: 5px;
  height: auto;
  filter: drop-shadow(0 0 0 #fd1853);
  z-index: -5;
  transition: all 0.8s ease;
}

button:hover .star-1 {
  position: absolute;
  top: -2%;
  left: 0%;
  width: 25px;
  height: auto;
  filter: drop-shadow(0 0 10px #fd1853);
  z-index: 2;
}

button:hover .star-2 {
  position: absolute;
  top: 34%;
  left: 41.5%;
  width: 15px;
  height: auto;
  filter: drop-shadow(0 0 10px #fd1853);
  z-index: 2;
}

button:hover .star-3 {
  position: absolute;
  top: 55%;
  left: 25%;
  width: 5px;
  height: auto;
  filter: drop-shadow(0 0 10px #fd1853);
  z-index: 2;
}

button:hover .star-4 {
  position: absolute;
  top: 0%;
  left: 55%;
  width: 8px;
  height: auto;
  filter: drop-shadow(0 0 10px #fd1853);
  z-index: 2;
}

button:hover .star-5 {
  position: absolute;
  top: 25%;
  left: 85%;
  width: 15px;
  height: auto;
  filter: drop-shadow(0 0 10px #fd1853);
  z-index: 2;
}

button:hover .star-6 {
  position: absolute;
  top: 75%;
  left: 60%;
  width: 5px;
  height: auto;
  filter: drop-shadow(0 0 10px #fd1853);
  z-index: 2;
}
</style>
