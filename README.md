<!DOCTYPE html>
<html Lang="pt-BR">
<cabeça>
    <meta conjunto de caracteres="UTF-8">
    <meta nome="Viewport" conteúdo="largura = largura do dispositivo, escala inicial = 1,0">
    <título>Coração de Fogo com Fogos</título>
    <estilo>
        corpo {
            exposição: flexionar;
            justificar-conteúdo: centro;
            alinhar itens: centro;
            altura: 100vh;
            margem: 0;
            cor de fundo: #000;
            transbordar: escondido;
        }
        lona {
            fronteira: 1Px sólido #333;
        }
    </estilo>
</cabeça>
<corpo>
    <lona id="heartCanvas" Largura="400" altura="400"></lona>
    <roteiro>
        Const lona = documento.getElementById('heartCanvas');
        Const CTX = lona.getContext('2d');

        Função para obter pontos do contorno do coração
        função Obter HeartPoints() {
            Const Pontos = [];
            Const Passos = 1000;
            durante (deixar t = 0; t <= 1; t += 1 / Passos) {
                Const x1 = 200 * Matemática.prisioneiro de guerra(Matemática.pecado(t * Matemática.PI * 2), 3);
                Const y1 = 13 * Matemática.Porque(t * Matemática.PI * 2) - 5 * Matemática.Porque(2 * t * Matemática.PI * 2) - 2 * Matemática.Porque(3 * t * Matemática.PI * 2) - Matemática.Porque(4 * t * Matemática.PI * 2);
 Pontos.empurrar({ x: 200 + x1, y: 220 - y1 * 10 });
            }
