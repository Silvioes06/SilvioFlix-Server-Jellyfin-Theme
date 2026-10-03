# SilvioFlix Jellyfin Theme

Tema escuro, moderno, elegante e minimalista para o Jellyfin do **SilvioFlix Media Server**.

## Identidade visual

- Fundo: preto/grafite muito escuro.
- Destaques: azul escuro e azul moderno.
- Logo: símbolo circular **SF** + texto **SilvioFlix / MEDIA SERVER**.
- Interface: bordas discretas, painéis escuros, navegação limpa e barras de progresso azuis.
- Pensado para um servidor NAS de mídia com biblioteca de vídeos.

## Estrutura

```text
SilvioFlix-Jellyfin-Theme/
├── assets/
│   └── img/
│       └── SilvioFlix-Logo.svg
├── css/
│   ├── default.css
│   └── main.css
├── AUTHORS
├── LICENSE.txt
└── README.md
```

## Instalação

1. Copie `css/default.css`, `css/main.css` e `assets/img/SilvioFlix-Logo.svg` para um local acessível ao Jellyfin.
2. No Jellyfin, abra **Dashboard → General → Custom CSS** (a localização pode variar conforme a versão).
3. Cole o conteúdo de `css/default.css` e `css/main.css`, ou mantenha-os juntos em um único arquivo CSS.
4. Garanta que o caminho relativo `../assets/img/SilvioFlix-Logo.svg` seja acessível pelo navegador do Jellyfin.
5. Salve e recarregue a interface.

### Alternativa simples

Se você preferir usar um único CSS, concatene:

```bash
cat css/default.css css/main.css > silvioflix-jellyfin.css
```

Depois cole `silvioflix-jellyfin.css` no campo de Custom CSS do Jellyfin.

## Yocto Project

O tema é independente da distribuição do servidor. Ele pode ser usado em um NAS que esteja executando uma imagem Linux construída com o **Yocto Project**, incluindo uma imagem personalizada para o SilvioFlix Media Server.

## Licença

Consulte `LICENSE.txt`.

## Autores

Consulte `AUTHORS`.
