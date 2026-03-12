<p align="center">
  <img src="logo.png" alt="Logo" width="320"/>
</p>

<h1 align="center">SlackBuilds para Slackware (Stable e Current)</h1>

<h3 align="center">Este repositório contém scripts *SlackBuild* personalizados
e atualizados para compilar e empacotar softwares de terceiros no Slackware Linux,
compatíveis tanto com as versões stable quanto current. 🐧</h3>

## 🌟 Objetivo

Fornecer scripts SlackBuild prontos para uso, com foco em:

* Manutenção de compatibilidade com Slackware **15.0** (stable) e **current**
* Correções de build para versões mais recentes de software
* Inclusão de patches e opções para ambientes modernos
* Scripts organizados, testados e documentados
* Esse repositório não será amplo, ele servirá para pacotes específicos que não
  serão mantidos via AppImage, como drivers, comandos não estáticos, etc;

## 🗂️ Organização

```
slackbuilds/
├— nome-do-pacote/
│   ├— nome-do-pacote.SlackBuild
│   ├— nome-do-pacote.info
│   ├— slack-desc
│   ├— README
│   └— patches/ (opcional)
└— ...
```

Cada diretório corresponde a um pacote individual. Para informações específicas sobre
dependências, uso ou peculiaridades do pacote, consulte o arquivo `README`
dentro do respectivo diretório.

## ⚙️ Como usar

1. Instale as dependências necessárias (indicadas no `.info` ou `README` de cada pacote).
2. Torne o script executável:

```bash
chmod +x nome-do-pacote.SlackBuild
```

3. Compile o pacote como root:

```bash
su
./nome-do-pacote.SlackBuild
```

4. Instale o pacote gerado com o `installpkg`:

```bash
installpkg /tmp/nome-do-pacote-*.txz
```

## ♻️ Compatibilidade

* ✅ Testado em Slackware 15.0 (stable)
* 🔄 Compatível com Slackware current (atualizações contínuas)
* 🧪 Alguns scripts possuem ajustes automáticos para versões diferentes

## 📦 Adicionando novos pacotes

1. Crie um diretório com o nome do pacote.
2. Inclua os seguintes arquivos obrigatórios:

   * `.SlackBuild`
   * `.info`
   * `slack-desc`
3. Opcionalmente, adicione:

   * `README`
   * `patches/` (com correções específicas)
4. Envie um *pull request* ou abra uma issue.

## 📜 Licença

Todos os scripts neste repositório estão licenciados sob a
[Licença Pública Geral GNU v2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html),
exceto quando indicado de outra forma nos diretórios individuais. 🧾

## 🙋 Contribuições

Contribuições, correções e melhorias são bem-vindas! Seja para atualizar scripts,
adaptá-los ao current, ou melhorar a documentação — toda ajuda é apreciada. 💪

Slackware: keep it simple, keep it Slack. 😎
 
