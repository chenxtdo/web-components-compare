<!-- your code here -->
<svelte:options tag="hello-component" />
<script >
import  './Hi.svelte'
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
<hi-component  first="Stencil" last="'Don't call me a framework' JS"></hi-component>
  