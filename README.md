<html>
  <form method="POST">
    <input type="text" name="angka1"/>
    <select name="operator">
      <option value="plus">+</option>
      <option value="minus">-</option>
      <option value="mult">X</option>
      <option value="div">/</option>
    </select>
    <input type="text" name="angka2"/>
    
    <input type="submit" name="submit" />
  </form>
</html>

<?php

if($_SERVER[REQUEST_METHOD"] == "POST"){
 $angka1 = $_POST('angka1');
 $angka2 = $_POST('angka2');
 $opertator = $_POST();

 echo $angka1;
 echo $angka2;
 echo $operator;

if($operator === "plus"){
 $result = $angka1 + $angka2;
 }
 else if($operator === "minus"){
 $result = $angka1 - $angka2;
 }

echo $result;
}



