# Changelog

## 1.0.5 — 2026-10-22

### Changed
- **No more PIN.** Kstrap no longer uses Windows Hello. Your saved accounts are encrypted by Windows for your Windows user: other users of the PC and copies of the files can't open them, but programs running as you could, as with any launcher that saves logins. If your accounts were saved under the PIN, Kstrap asks for it **one last time** to move them, then never again.
- **Faster game launch with a preferred server region.** The region search used to run up to 7 seconds and then pick nothing. It now gives up within 3 seconds, stops at the first open server it finds in your region, runs while the rest of the launch is prepared, and writes in the log why when it picks nothing.
- Browser links no longer look up the profile's outfits online before handing the launch to the open Kstrap window.

### Added
- **Start in 3 steps** for new users: add an account, create a profile for it, and make the website's Play button open through Kstrap. Close it with × if you don't need it.
- **Delete profile** is now in the profile's right-click menu in the sidebar and as a bin icon on the profile page (it was hidden at the bottom of Advanced). A profile that is playing can't be deleted until its Roblox closes.
- After 10 hours of play through Kstrap, the footer asks once whether you'd like to support it on Ko-fi. Close it and it never comes back.

**Português (pt-BR)**

### Mudou
- **Sem PIN.** O Kstrap não usa mais o Windows Hello. Suas contas salvas ficam criptografadas pelo Windows pro seu usuário: outros usuários do PC e cópias dos arquivos não conseguem abrir, mas programas rodando como você conseguiriam, como em qualquer launcher que salva login. Se suas contas estavam salvas com PIN, o Kstrap pede ele **uma última vez** pra passar elas pro novo formato, e nunca mais.
- **Jogo abre mais rápido com região de servidor preferida.** A busca de região levava até 7 segundos e não escolhia nada. Agora ela desiste em até 3 segundos, para no primeiro servidor livre que achar na sua região, roda enquanto o resto do lançamento é preparado e escreve no log o motivo quando não escolhe nenhum.
- Links do navegador não buscam mais as roupas do perfil na internet antes de passar o lançamento pra janela do Kstrap aberta.

### Adicionado
- **Comece em 3 passos** pra quem é novo: adicionar uma conta, criar um perfil pra ela e fazer o Jogar do site abrir pelo Kstrap. Feche no × se não precisar.
- **Excluir perfil** agora fica no menu do botão direito do perfil na barra lateral e num ícone de lixeira na página do perfil (estava escondido no fim de Avançado). Um perfil que está jogando só pode ser excluído depois que o Roblox dele fechar.
- Depois de 10 horas de jogo pelo Kstrap, o rodapé pergunta uma vez se você quer apoiar no Ko-fi. Fechou, não volta.

## 1.0.4 — 2026-10-22

### Added
- **About › AI integration** now has an on/off switch. Off: AI tools can't start Kstrap's AI integration, and a session that was already open answers "turned off" once and then closes, so nothing of Kstrap's keeps running for it. On by default.
- *Copy AI instructions* is disabled while the switch is off.

**Português (pt-BR)**

### Adicionado
- **Sobre › Integração com IA** agora tem um botão de ligar/desligar. Desligada: as ferramentas de IA não conseguem iniciar a integração do Kstrap, e uma sessão que já estava aberta responde "desligada" uma vez e fecha, então nada do Kstrap fica rodando pra ela. Vem ligada.
- *Copiar instruções pra IA* fica desativado enquanto ela está desligada.

## 1.0.3 — 2026-10-22

### Fixed
- After updating from 1.0.1 to 1.0.2, the "what changed" notice never appeared. Updating from any older version now shows it.
- Release notes no longer show stray `*` marks.

### Added
- **About › What's new in this version** opens the notes of the version you're running, any time.
- Release notes now come in English and Portuguese; Kstrap shows the one in its language.
- The notes dialog links to the full changelog, so if you skipped a version you can see everything you missed.

**Português (pt-BR)**

### Corrigido
- Depois de atualizar da 1.0.1 pra 1.0.2, o aviso "o que mudou" não aparecia. Agora aparece ao atualizar de qualquer versão anterior.
- As notas de versão não mostram mais asteriscos soltos.

### Adicionado
- **Sobre › O que mudou nesta versão** abre as notas da versão que você está usando, a qualquer hora.
- As notas de versão agora vêm em inglês e português; o Kstrap mostra a do idioma dele.
- O diálogo das notas tem link pro histórico completo, então quem pulou uma versão vê tudo o que perdeu.

## 1.0.2 — 2026-10-21

### Added
- **Local API switch** (About › Local API). On by default. Turning it off means nothing listens on your PC, but every browser link then asks for your Windows PIN.
- **AI integration (MCP)** is now included. It is **off until you add it to an AI tool yourself**: About › AI integration › *Copy AI instructions* gives you the setup command and short rules for the AI. It runs only while that AI tool is open and talks to it through a local pipe, with no open port. Like the app, it contacts Roblox to do what the AI asks (for example, listing servers also uses ipinfo.io and apis.rovalra.com; see the README).
- **What's new**: when an update is ready, the footer links to its notes. After updating, the footer says which version you're on and links to what changed. This starts working from the next update on.

### Changed
- The README now lists every service Kstrap talks to and what is stored on your PC.

## 1.0.1 — 2026-10-20

### Fixed
- Opening a game from the browser could sit on the first step for up to 5 minutes. When the launch failed inside the open Kstrap window, the error never reached the picker. Every error now comes back right away, with a readable message.

### Added
- A local log at `%LocalAppData%\Kstrap\logs\kstrap.log` with how long each launch step took and any errors, so slow or failed launches can be traced. Login cookies and tickets are removed before anything is written.

## 1.0.0 — 2026-10-19

First public release.

### Added
- Profiles: each one has its own account, outfit, FastFlags, mods, Roblox version, FPS cap and server region.
- Wardrobe: your account's saved outfits; the one you pick is worn when the profile opens a game.
- Several Roblox windows at once, each with its own profile.
- Profile picker when you click **Play** on roblox.com, with an outfit choice just for that match and a step-by-step launch.
- Play time, sessions and a play-style hexagon per profile (counted from now on, while Kstrap is running).
- Preferred server region, auto-rejoin, Performance / Balanced / Quality templates.
- Accounts encrypted on your PC and protected by Windows Hello.
- English and Português (Brasil); automatic updates.
