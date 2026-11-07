# Horto Ville 3 | Klebson Souza

Landing page simples para anúncios do Facebook/Instagram. O visitante vê as fotos do empreendimento, confere os dados do corretor e clica em um botão que abre o WhatsApp com uma mensagem pronta.

**Corretor:** Klebson Souza, Corretor de Imóveis
**CRECI:** CRECI-BA 37964

## Arquivos

| Arquivo | Para que serve |
|---|---|
| `index.html` | A página inteira (visual, carrossel e link do WhatsApp) |
| `entrada.jpg` | Foto da portaria |
| `esporte.jpg` | Foto da quadra esportiva |
| `playground.jpg` | Foto do playground |
| `pets.jpg` | Foto do espaço pet |
| `klebson.jpg` | Foto do corretor |

Todos os arquivos precisam ficar juntos, na raiz do repositório.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (por exemplo, `horto-ville-3`).
2. Envie todos os arquivos desta pasta para a raiz do repositório.
3. Vá em **Settings**, depois **Pages**.
4. Em **Source**, escolha **Deploy from a branch**, selecione a branch `main` e a pasta `/ (root)`, e clique em **Save**.
5. Aguarde cerca de 1 a 2 minutos. O link aparece na mesma tela e fica assim:
   `https://SEU-USUARIO.github.io/horto-ville-3/`
6. Use esse link como destino do anúncio.

## Como editar

### Número e mensagem do WhatsApp

No final do `index.html`, procure o bloco abaixo e altere o que precisar:

```js
var WHATSAPP = "5575982193793";
var MENSAGEM = "Olá, Klebson! Vi o anúncio do Horto Ville 3 e quero receber os valores e condições.";
```

O número deve ter só dígitos: 55 (Brasil) + DDD + número.

### Texto do botão

Procure por `Quero receber valores e condições` no `index.html` e troque pelo texto desejado. A linha menor ("Resposta direta pelo WhatsApp") fica logo abaixo.

### Fotos do carrossel

Troque os arquivos `.jpg` mantendo o mesmo nome, ou edite o bloco `<div class="track">` no `index.html` para adicionar ou remover slides. Cada slide tem um `data-label`, que é o texto da legenda exibida sobre a foto.

## Pixel do Facebook (opcional)

1. No `index.html`, localize o comentário `META PIXEL (opcional)` dentro do `<head>`.
2. Cole ali o código base do seu Pixel.

Com o Pixel instalado, cada clique no botão do WhatsApp registra automaticamente o evento `Contact`, que pode ser usado para medir e otimizar o anúncio.

## Observações

- A página usa a fonte Manrope, do Google Fonts. Se ela não carregar, o navegador usa uma fonte padrão do sistema.
- O carrossel passa sozinho a cada 4 segundos e pode ser deslizado com o dedo. Quem usa o modo de movimento reduzido no aparelho não vê a troca automática.
- As imagens do empreendimento pertencem aos seus respectivos responsáveis (realização ABS e coordenação Affonso Henriques). Use-as apenas com autorização.
