<!-- your code here -->
<svelte:options tag="hi-component" />
<script >

 export let first;
 export let middle; 
 export let last;

 function format(first, middle, last) {
  return (first || '') + (middle ? ` ${middle}` : '') + (last ? ` ${last}` : '');
}

function getText() {
   console.log(first, middle, last);
   return first + middle + last;
 }


  </script>
  <style>
      
  </style>
  <div>Hi, World! I'm {first} {getText()}</div>