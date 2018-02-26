# fb-image.js
corrige orientação de imagem digital

# uso:

`js
resetOrientation(this, function(imgCorrigida, imgOriginal){
  //exibe a foto tirada em uma tag <img id="image-id">
  $("#image-id").attr("src", imgCorrigida);
  //colocar o base64 retornado no textarea
	$("#textarea-id").val(imgCorrigida);
  });	
`
