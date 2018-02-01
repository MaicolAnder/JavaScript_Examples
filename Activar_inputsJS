//Activar o desactivar input HTML al seleccionar (<option value='Elemento'></option>) de un select

$("#elemento_que_activa").change(activador);
function activador(){ 
	var item_selected=$("#elemento_que_activa option:selected").text();
	if (item_selected=='Elemento') {
        $('#elemento_a_activar').prop('disabled', false);
      }else{
        $('#elemento_a_activar').prop('disabled', 'disabled');
      }
}

//Miguel A. Tunubalá.
