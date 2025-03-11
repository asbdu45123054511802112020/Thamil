<div class="ring-container">
  <div class="butterfly-ring">
    <p id="name1">Sakthi</p>
    <p id="name2">Anandhi</p>
  </div>
</div>
```

CSS:

```
.ring-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #f0f0f0;
}

.butterfly-ring {
  position: relative;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  background-color: #fff;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

#name1, #name2 {
  position: absolute;
  font-size: 24px;
  font-family: Arial, sans-serif;
  color: #666;
}

#name1 {
  top: 50%;
  left: 20%;
  transform: translate(-50%, -50%);
}

#name2 {
  top: 50%;
  right: 20%;
  transform: translate(50%, -50%);
}

.butterfly-ring:before {
  content: "";
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 50px;
  height: 20px;
  background-color: #fff;
  border-radius: 50%;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.butterfly-ring:after {
  content: "";
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 20px;
  height: 50px;
  background-color: #fff;
  border-radius: 50%;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
```
