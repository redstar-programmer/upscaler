# Redstar upscaler
Ferramenta poderosa de upscaling de vídeo usando FFmpeg, Real-ESRGAN, Flowframes - agora suporta **IU multilíngue**!

🌐 Idioma:
[Inglês](README.en.md) | [Coreano](README.md) | [日本語](README.ja.md) | [中文](README.zh.md) | [日本語](README.ja.md)
[Français](README.fr.md) | [Deutsch](README.de.md) | [Español](README.es.md) | [Português](README.pt.md) |
[Русский](README.ru.md) | [Italiano](README.it.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) |
[ภาษาไทย](README.th.md) | [العربية](README.ar.md)

<p align="centre">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="centre">
  <strong>Ferramenta de upscaling de vídeo baseada em fmpeg, realesrgan, flowframes</strong><br>
  <em>Moderna GUI baseada, configurações pré-definidas, suporte para processamento de múltiplos arquivos</em>
</p>

---.

Descarregar: [Release](https://github.com/redstar-programmer/upscaler/releases/)

## ✨ Por favor, suporte o upscaler 'redstar'

Você gosta deste projeto ou quer apoiar o seu desenvolvimento?
Faça uma pequena doação para nos ajudar a construir melhores recursos e atualizações confiáveis!

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**Patrocinadores do GitHub** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡 O vosso patrocínio dos custos do servidor, do tempo de desenvolvimento e de uma chávena de café é muito importante. Obrigado!

## Índice

- [👋 Introdução](#Introdução)
- [💾 Instalação e preparação](#Instalação-e-Preparação)
- [🔧 Caraterísticas principais](#Caraterísticas principais)
- 🚀 Como utilizar (Início rápido)](#Comoutilizar-o-início-rápido)
- [⚙️ Descrição pormenorizada das caraterísticas](#descrição-detalhada-das-caraterísticas)
- [🙏 Agradecimentos](#Agradecimentos)
- 📜 História](#história)

## 👋 Introdução
O upscaler da **redstar é uma ferramenta GUI baseada em Python para fazer o upscale automático de vídeos para resoluções mais altas usando `ffmpeg`, `Real-ESRGAN` e `Flowframes`.

- Extrai quadros de vídeo → upscale → mescla vídeo em uma única etapa
- Suporta vários modelos de realesrgan
- Interpolação opcional via Flowframes
- Extração e processamento automáticos de codecs de áudio
- Trabalha na localização da fonte ou num caminho especificado

> ⚠️ Desenvolvido e testado num ambiente Windows.

Abaixo está uma simples demonstração de uso:<br>
![미디어1](https://github.com/user-attachments/assets/ba601a08-6749-45fd-ae21-f1a2a52987f6)

## 💾 Instalação e preparação

1. Instale e localize as seguintes ferramentas externas (note que o ficheiro de distribuição inclui os instaladores do ffmpeg, Real-ESRGAN e Flowframes (consulte a pasta Programas no caminho))
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - [Flowframes](https://github.com/n00mkrad/flowframes) *(opcional)*.
2. descompactar e executar o upscaler.exe da readstar
3. no caso do Flowframes, os modelos carregados podem ser diferentes, dependendo do seu ambiente, portanto, certifique-se de executar o Flowframes e de que o AI de interpolação e o modelo AI na guia Interpolação correspondem à versão de resources/flowframes_models.ini do upscaler da redstar. <br>Comente os modelos que não estão carregados marcando-os com # e certifique-se de que a ordem dos modelos na janela de configurações do upscaler da redstar corresponda à ordem dos modelos no <br>Flowframes antes de prosseguir.

## 🔧 Principais caraterísticas.

![Image](https://github.com/user-attachments/assets/072af636-e967-4e4b-b194-33b96f580780)
- Seleção múltipla de vídeo e operação sequencial
- Adicionar vídeo por arrastar e largar
- Disponibilidade do programa principal e seleção direta
- Modo de poupança de disco
- Suporte multilingue (15 idiomas)
<br><br>
![Image](https://github.com/user-attachments/assets/23dd7e8a-0e01-409f-b162-a9512fda09fc)
- Guardar e aplicar automaticamente predefinições
- Deteção automática de codecs de áudio e definição de taxa de bits
- Deteção e seleção automáticas de modelos de realesrgan
- Configurações detalhadas para FFMPEG, real-ESRGAN e Flowframes
- Alterar as definições das opções de acordo com a versão do Flowframes<br>(A versão pode ser alterada especificando o caminho da versão no flowframes na página principal)
<br><br>
![Image](https://github.com/user-attachments/assets/ab7d9410-1fb4-450b-92d5-56a6d583a64c)
- ✅ Verificar o comando de execução do upscale (pode ser copiado e executado separadamente no CMD)
<br><br>
![Image](https://github.com/user-attachments/assets/4898904a-bb23-4dba-997d-23ca744fed93)
- Monitorizar o progresso geral da operação de aumento de escala
- Verificar o registo de upscale (os ficheiros de registo são criados por data na pasta de registo na pasta live)
- Limpar automaticamente os resultados após a conclusão do trabalho (prefixados com [REDSTAR])
- Definir a ação após a conclusão da tarefa<br>(Não fazer nada / Sair do programa / Modo de suspensão / Modo de hibernação / Fechar janela)
<br><br>
## 🚀 Como utilizar (Início rápido)

1. adicionar ficheiros de vídeo (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV suportados)
2. especifique o local de trabalho ou assinale a caixa "Use original file path" (Utilizar caminho do ficheiro original)
3. clicar no botão "Settings" (Definições) no vídeo adicionado
4. definições detalhadas do ffmpeg, realESRGAN, Flowframes
5. clicar em Batch apply to all files / Apply to selected files only
6. clicar no botão "Confirm" (Confirmar)
7. verificar os comandos a executar e clicar no botão "Start Task

> O resultado da tarefa serão dois ficheiros: vídeo melhorado e vídeo interpolado na pasta selecionada.
> ✨ Os ficheiros concluídos serão guardados com o prefixo [REDSTAR].
---]

## ⚙️ Descrição pormenorizada da função

| Item | Descrição |
|------|------|
| Definir caminho de trabalho** | Fornecer caminho padrão ou opção "Usar caminho do arquivo original" |
| Suporte de formato de vídeo** | A maioria dos formatos suportados, incluindo MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV, etc.
| Detecta automaticamente realesr-animevideov3, realesr-general, 4xplus, etc.
| Processamento de áudio** | Suporte para codificação de vários formatos, como `aac`, `mp3`, `flac`, etc.
| Integração de quadros de fluxo** | Interpolação (FPS ×2, ×4, ×8) pode ser definida
| Modo de poupança de disco** | Eliminação automática de imagens intermédias

## Agradecimentos

- realesrgan por [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes por [n00mkrad](https://github.com/n00mkrad/flowframes)
- Se quiser contribuir para este projeto ou sugerir uma funcionalidade, por favor deixe um comentário em [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues).

# 📜 História

v 1.1.0
 > 1. configuração do menu (abrir ficheiro, fechar ficheiro, definições de registo, definições de idioma)
 > 2. Definições de vários idiomas adicionadas (idiomas disponíveis: Coreano, Inglês, 日本語, 中文, Français, Deutsch, Español, Português, Русский, Tiếng Việt, Bahasa Indonesia, ไทย, Italiano, العربية)
 > 3. mensagens alteradas e algum código para acomodar as definições de idioma adicionadas
 > 4. algumas alterações na configuração da IU
 > 5. informação da versão do ffmpeg, real-ESRGAN, Flowframes apresentada (ecrã principal)
 > 6. suporte para a versão 1.41.0 do Flowframes (atualmente só estão disponíveis as versões 1.40.0 e 1.36.0 devido a um problema com o comando cmd na versão 1.41.0)
 > 7. corrigido um problema em que os itens do AI Models eram apresentados em letras minúsculas
 > 8. adicionadas opções FFMPEG (Pixel, codec de vídeo) - as opções são apresentadas de acordo com o PC do utilizador
 > 9. verificação CUDA melhorada para o PC de cada utilizador - verificar a disponibilidade e o tipo de GPU (ecrã principal)

v 1.0.0
 > 1. reescrita completa do código
 > 2. alterações na IU
 > 3. aumento da gama de vídeo/áudio que pode ser processado
 > 4. adicionado o modo de poupança de disco
 > 5. distribuição incluindo os principais programas

v 0.1.92
 > 1. corrigido um problema que fazia com que a interpolação falhasse devido a entradas duplicadas na caixa combinada do modelo AI quando se alterava o caminho dos quadros de fluxo.
 > 2. adicionado um código de verificação para o estado de seleção da caixa combinada durante a interpolação.

v 0.1.91
 > 1. adicionadas algumas funções de atualização da caixa combinada relacionadas com o Flowframes
 > 2. ajustados alguns ficheiros de distribuição

v 0.1.9
 > 1. aplicar alterações ao modelo Flowframes
 > 2. novo modelo Flowframes 1.36.0, implementação do modelo 1.40.0
 > 3. falha na linha de comando do Flowframes não ocorre mais
 > 4. os ficheiros podem agora ser adicionados arrastando/soltando
 > 5. corrigido o facto de as definições do Flowframes não serem aplicadas

v 0.1.8
 > 1. corrigido o erro de verificação da nova versão ao verificar a versão
 > 2. se o flowframes estiver instalado no caminho predefinido (ex. C:\Users\Administrador\AppData\Local\Flowframes\), defina o caminho como predefinido antes de iniciar.
 > 3. Ao adicionar várias selecções de ficheiros, a aplicação falha devido a um erro.
 > 4. corrigido um erro ao iniciar a tarefa depois de adicionar vários ficheiros

v 0.1.7
 > 1. o tamanho do programa pode ser alterado
 > 2. corrigido um erro ao trabalhar com ficheiros sem voz
 > 3. Alterada toda a configuração da IU (reconfigurada para se adaptar à alteração do tamanho)

v 0.1.6
 > 1. corrigido um problema com diferentes tamanhos de letra dependendo da resolução do ecrã
 > 2. corrigido um problema em que o título do programa não mostrava a informação da versão como uma nova versão
 > 3. foi corrigido um problema em que o ficheiro config.ini era guardado num caminho diferente
 > 4. ao alterar o multiplicador de aumento de escala realesrgan, a caixa de combinação do modelo de aumento de escala também é alterada.
 > 5. adicionada a função de verificação de atualização
 > 6. corrigida alguma lógica
 > 7. cor alterada das tabelas de resolução e fps
 > Permitir ao utilizador editar a resolução (tem de ser introduzida como 1024x768)

v 0.1.5
 > 1. corrigido um problema em que o modelo AI não era automaticamente alterado quando se seleccionava a interpolação AI FLOWFRAMES
 > 2. corrigido um problema em que a interpolação de quadros de fluxo não era interpolada de acordo com a opção selecionada
 > 3. adicionada a caixa de combinação "Método de cálculo de FPS" para evitar o cálculo incorreto de FPS para alguns vídeos.
        -> r_frame_rate / avg_frame_rate, a predefinição é r_frame_rate
 > 4. Mostrar o progresso da obtenção de informações de vídeo ao selecionar um ficheiro de vídeo
 > 5. alterar a predefinição para abrir a última pasta selecionada ao selecionar um ficheiro novamente após a abertura do ficheiro

v 0.1.4
 > 1. Alterada a forma como o ficheiro config.ini é lido
 > 2. alterada a forma de obter informação de vídeo do Python AV para o ffmpeg
 > 3. adicionada janela de fecho quando a tarefa está terminada
 > 4. mostrar o nome completo do ficheiro como dica de ferramenta ao passar o rato na lista de tarefas
 > 5. Mostrar resolução(antes) / resolução(depois) / FPS(antes) / FPS(depois) para cada ficheiro na lista de tarefas
 > 6. remover a caixa de entrada FPS (devido à rotulagem acima para cada ficheiro)
 > 7. remover o tamanho estimado do FPS de saída (removido devido à rotulagem específica do ficheiro acima)
 > 8. mostrar o progresso como duas barras de progresso para todos os ficheiros/trabalhos

v 0.1.3
 > 1. corrigido o erro de cálculo do FPS do ficheiro em que algumas informações de FPS estavam erradas ao carregar ficheiros

v 0.1.2
 > 1. alterações na configuração da interface do utilizador
 > 2. mudanças na lógica interna
 > 3. corrigido o problema em que o modelo realesrgan não funcionava quando se seleccionavam dois dos seguintes modelos
 > 4. alteração da forma de utilizar os modelos realesrgan
 > -> Copie o novo ficheiro de modelo (*.param) para a pasta de modelos na pasta de instalação do realesrgan e pode utilizá-lo.
 > 5. mostrar a informação sobre a largura, altura e tamanho estimado do último ficheiro da imagem alvo com que trabalhar
 > 6. escrever o código para migrar o ficheiro config.ini
 > 7. alterar a imagem de decomposição FFMPEG AAC -> FLAC
 > 8. outras correcções de erros

v 0.1.1
 > 1. primeira vez que escrevo um programa de upscaling de vídeo com ffmepg, realesrgan e flowframes