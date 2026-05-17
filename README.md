# ⚡ ClipMaker - AI Viral Moments

<p align="center">
  <img src="https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white" alt="Gemini">
  <img src="https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white" alt="Cloudinary">
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind">
</p>

O **ClipMaker** é uma aplicação web experimental que utiliza Inteligência Artificial para identificar automaticamente os momentos mais engajadores (virais) em vídeos, realizando o corte de forma inteligente.

Este projeto foi desenvolvido durante a trilha de Inteligência Artificial da **NLW (Next Level Week)** da Rocketseat.

## 🚀 Funcionalidades

- **Upload de Vídeo:** Integração direta com o Cloudinary para upload e armazenamento.
- **Transcrição Automática:** Utiliza o serviço do Cloudinary para converter áudio em texto.
- **Análise com IA:** Integração com o Google Gemini (1.5 Flash) para analisar a transcrição e decidir os melhores tempos de início e fim do clipe.
- **Edição On-the-fly:** Utiliza as transformações de URL do Cloudinary para entregar apenas o trecho viral selecionado pela IA.
- **Interface Fluida:** Animações modernas feitas com GSAP e estilização com Tailwind CSS.

## 🛠️ Tecnologias Utilizadas

- [Google Gemini API](https://aistudio.google.com/) (Modelo 1.5-Flash)
- [Cloudinary](https://cloudinary.com/) (Upload Widget & Video Transformations)
- [Tailwind CSS](https://tailwindcss.com/) (Estilização)
- [GSAP](https://greensock.com/gsap/) (Animações)
- [Lucide Icons](https://lucide.dev/) (Ícones)

## ⚙️ Como Configurar

Para rodar este projeto localmente, siga os passos abaixo:

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   ```

2. **Configuração do Cloudinary:**
   - Crie uma conta no [Cloudinary](https://cloudinary.com/).
   - No seu Dashboard, encontre o seu `Cloud Name`.
   - Vá em *Settings > Upload* e crie um `Upload Preset` do tipo **Unsigned**.
   - Certifique-se de habilitar a geração de transcrições no preset ou via configurações da conta.
   - No arquivo `index.html`, substitua os valores de `cloudName` e `uploadPreset` pelas suas credenciais.

3. **Obtenha uma API Key do Gemini:**
   - Acesse o Google AI Studio.
   - Crie uma nova API Key.

4. **Execução:**
   - Basta abrir o arquivo `index.html` em qualquer navegador moderno.
   - Insira sua chave do Gemini na interface do usuário antes de iniciar o upload.

## 🔒 Segurança

Este projeto foi construído para que a chave da API do Gemini seja inserida via interface pelo usuário e não fique exposta no código-fonte. **Nunca suba suas chaves privadas para o GitHub.**

---
Desenvolvido com 💜 por [ Atawan Cazetta ] durante a NLW da Rocketseat.