<!-- your code here -->
<svelte:options tag="my-component" />
<script >
 export let first;
 export let middle; 
 export let last;

 function format(first, middle, last) {
  return (first || '') + (middle ? ` ${middle}` : '') + (last ? ` ${last}` : '');
}

 function getText() {
   return format(first, middle, last)
 }


  </script>
  <style>
      
  </style>
  <div>Ni, Hao! I'm {getText()}</div>