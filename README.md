# texto-em-voz-javascript-puro
##transformar texto em voz com javascript puro


function fale(texto) {
    let msg = texto
    
    let speech = new SpeechSynthesisUtterance();
    speech.lang = "pt-br";
    
    speech.text = msg;
    speech.volume = 1;
    speech.rate = 1;
    speech.pitch = 1;
    
    window.speechSynthesis.speak(speech);
}

function falar(texto){
    fale(texto)
}
