function sumar_fecha(fecha, intervalo, dma, separador) {
    // sumar_fecha("2017-01-01", "+-5", "d m a");
    var separador = separador || "-";
    var arrayFecha = fecha.split(separador);
    var dia = arrayFecha[2];
    var mes = arrayFecha[1];
    var anio = arrayFecha[0];  
     
    var fechaInicial = new Date(anio, mes - 1, dia);
    var fechaFinal = fechaInicial;
    if(dma=="m" || dma=="M"){
        fechaFinal.setMonth(fechaInicial.getMonth()+parseInt(intervalo));
    }else if(dma=="y" || dma=="Y"){
        fechaFinal.setFullYear(fechaInicial.getFullYear()+parseInt(intervalo));
    }else if(dma=="d" || dma=="D"){
        fechaFinal.setDate(fechaInicial.getDate()+parseInt(intervalo));
    }else{
        return fecha;
    }
    dia = fechaFinal.getDate();
    mes = fechaFinal.getMonth() + 1;
    anio = fechaFinal.getFullYear();

    dia = (dia.toString().length == 1) ? "0" + dia.toString() : dia;
    mes = (mes.toString().length == 1) ? "0" + mes.toString() : mes;

    return dia + "-" + mes + "-" + anio;
}

function resta_fechas(f1,f2){
    // 2017-01-30
    var aFecha1 = f1.split('-');
    var aFecha2 = f2.split('-');
    var fFecha1 = Date.UTC(aFecha1[0], aFecha1[1]-1, aFecha1[2]);
    var fFecha2 = Date.UTC(aFecha2[0], aFecha2[1]-1, aFecha2[2]);
    var dif = fFecha2 - fFecha1;
    var dias = Math.floor(dif / (1000 * 60 * 60 * 24));
    return dias;
}
