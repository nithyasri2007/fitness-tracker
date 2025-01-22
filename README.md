# fitness-tracker
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Fitness tracker</title>
        <style>
            header h1{
                  text-align :center;
                  font-family: Georgia, 'Times New Roman', Times, serif;
                  font-display:unset;
            }
            header p{
                text-align: right;
                font-size: 20px ;
            }
            button{
                height :auto;
                width :auto;
            }
            
        </style>
    </head>
    <body>
        <header>
            <h1>FITNESS TRACKER</h1>
            <p>Be fit be healthy!</p>
        </header>
        <div class="container">
            <form id="fittness form">
                <div class="date">
                    <label for="date">Date:</label> 
                    <input type="date" id="date" required>
                </div><br>
                <div class="form-group">
                    <label for="steps">Steps taken:</label>
                    <input type="number" id="steps" placeholder="Enter steps" required>
                </div><br>
                <div class="form-group">
                    <label for="calories">Calories burned :</label>
                    <input type="number" id="calories" placeholder="EnterCalories" required>
                </div><br>
                <div class="form-group">
                    <label for="workout time">Workout duration(min):</label>
                    <input type="number" id="workout time" placeholder="workout timing" required>
                </div><br>
                <button type="button" onclick="adddate">Add activity</button><br><br>
                <div class="tracker output" id="output">
                    <h3>Your fitness activity :</h3>
                </div>
            </form>
            <script>
                function add fitnessdate(){
                    const date=document.getElementById('date').value;
                    const steps=document.getElementById('steps').value;
                    const calories=document.getElementById('calories').value;
                    const workout time=document.getElementById('workout time').value;
                      if(!date || !steps|| !calories ||!duration)
                      {
                        alert("Fill in all fields:")
                        return ;
                      }
                      const actiitylist=document.getElementById('activitylist');
                      const listitem=document.getElementById('activitylist');
                      const listitem=document.createElement('li');
                      listitem.textcontent='date': ${date},'steps':${steps},'calories' :${calories},'workout time' :${workout time}mins;
                      activitylist.appendchild(listItems);
                      document.getElementById('fitness-form').reset();
                }
            </script>
        </div><br>
        <footer>Copy@2024 All rights reserved.</footer>
    </body>
</html>
