# Quiz

<div id="quiz">
  <h3>Question 1:</h3>
  <p>Qual a universidade que mais acaba com sua vida?</p>
  <input type="radio" name="q1" value="Unama"> Unama<br>
  <input type="radio" name="q1" value="Famaz"> Famaz<br>
  <input type="radio" name="q1" value="Cesupa"> Cesupa<br>

  <button onclick="checkAnswers()">Submit</button>
  <p id="result"></p>
</div>

<script>
  function checkAnswers() {
    var correct = 0;
    var q1 = document.querySelector('input[name="q1"]:checked');
    if (q1 && q1.value === 'Cesupa') {
      correct++;
    }

    document.getElementById('result').innerText = "You acertou!!! Obteve " + correct + " de 1 resposta correta.";
  }
</script>