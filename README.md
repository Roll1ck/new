<!DOCTYPE html>
<html>
<body>
  <script>
function bubbleSort(arr) {
      var len = arr.length;
      for (var i = 0; i < len ; i++) {
        for(var j = 0 ; j < len - i - 1; j++){ 
        if (arr[j] > arr[j + 1]) {
          // swap
          var temp = arr[j];
          arr[j] = arr[j+1];
          arr[j + 1] = temp;
        }
       }
      }
    return arr;
  }
document.writeln(bubbleSort([7,5,2,4,3,9])); //[2, 3, 4, 5, 7, 9]
document.writeln(bubbleSort([9,7,5,4,3,1])); //[1, 3, 4, 5, 7, 9]
document.writeln(bubbleSort([1,2,3,4,5,6])); //[1, 2, 3, 4, 5, 6]
  </script>
</body>
</html>
