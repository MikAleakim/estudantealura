deixe palavra;

função setup() { createCanvas(400, 400);

palavra = palavraAleatória(); }

function palavraAleatoria(){ let palavras = ["Caminhante", "Caminho", "Caminha"]; return aleatório(palavras); }

função inicializaCores() {

fundo("branco"); preenchimento("preto"); tamanhodotexto(64); alinhamentodotexto(CENTRO, CENTRO); }

function palavraParcial(minimo, maximo) { let quantidade = map(mouseX, minimo, maximo, 1, palavra.length); deixe parcial = palavra.substring(0, quantidade); devolução parcial; }

função desenhar() {

inicializaCores();

deixe texto = palavraParcial(0, largura); texto(texto, 200, 200); }
