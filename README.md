body {
  margin: 0;
  padding: 0;
  overflow: hidden;
  font-family: Arial, sans-serif;
  background-color: #222;
}
canvas.game {
  display: block;
  width: 100vw;
  height: 100vh;
}
#score {
  position: fixed;
  top: 10px;
  left: 50%;
  transform: translateX(-50%);
  font-size: 2rem;
  color: white;
  font-weight: bold;
  z-index: 10;
  text-shadow: 0 0 5px #000;
}
#result-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0,0,0,0.7);
  display: flex;
  align-items: center;
  justify-content: center;
  visibility: hidden;
  z-index: 20;
}
#result {
  background-color: #fff;
  padding: 2rem 3rem;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 0 15px #000;
}
#result h1 {
  font-size: 2rem;
  margin-bottom: 1rem;
}
#result p {
  font-size: 1.2rem;
  margin-bottom: 1.5rem;
}
#retry {
  font-size: 1rem;
  padding: 0.5rem 1.5rem;
  border: none;
  border-radius: 8px;
  background-color: #2196f3;
  color: white;
  cursor: pointer;
}
#retry:hover {
  background-color: #1976d2;
}
#controls {
  position: fixed;
  bottom: 20px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  flex-direction: column;
  align-items: center;
  z-index: 10;
}
#controls div {
  display: flex;
  justify-content: center;
}
#controls button {
  width: 50px;
  height: 50px;
  font-size: 1.5rem;
  margin: 5px;
  border: none;
  border-radius: 10px;
  background-color: #555;
  color: white;
  cursor: pointer;
  transition: background-color 0.2s;
}
#controls button:active {
  background-color: #999;
}
@media (max-width: 600px) {
  #score { font-size: 1.5rem; }
  #controls button { width: 40px; height: 40px; font-size: 1.2rem; }
  #result { padding: 1.5rem 2rem; }
  #result h1 { font-size: 1.5rem; }
  #result p { font-size: 1rem; }
}