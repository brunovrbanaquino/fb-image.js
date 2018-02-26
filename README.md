# fb-image.js
corrige orientação de imagem digital

# uso:

```js
resetOrientation(this, function(imgCorrigida, imgOriginal){
  //exibe a foto tirada em uma tag <img id="image-id">
  $("#image-id").attr("src", imgCorrigida);
  //colocar o base64 retornado no textarea
	$("#textarea-id").val(imgCorrigida);
  });	
```

```html
<div>
<script src="fb-image.js"></script>
<form>
  <input type="file" id="teste" />
  <img src="" id="image-id" width="400px">
</form>
<script>
document.getElementById('teste').onchange = function(){
resetOrientation(this, function(imgCorrigida, imgOriginal){
  //exibe a foto tirada em uma tag <img id="image-id">
  document.getElementById('image-id').src = imgCorrigida

  //colocar o base64 retornado no textarea
	//$("#textarea-id").val(imgCorrigida);
  })	
}
</script>
</div>
```

