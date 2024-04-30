[comment]: <> (Links de referência)
[link]: https://
[link]: https://
[link]: https://

[comment]: <> (Banner)
<div align="center">
    <img src="https://github.com/Harlocks/design/blob/main/assets/figma/banners/VPS-BannerLogo.png?raw=true">
</div>

[comment]: <> (Separator)

<img src="https://github.com/Harlocks/design/blob/main/assets/figma/separators/VPS-Separator.png?raw=true">
<h3>
    <img src="https://github.com/Harlocks/design/blob/main/assets/inkscape/icons/apply.png?raw=true">
    Objetivo
</h3>

> Este guia tem como objetivo mostrar para o usuário que não é apenas comprar uma VPS e deixar ela executando. É necessário a busca pela segurança de seus dados, juntamente com todas as informações que estão armazenadas dentro da sua VPS. Lembrando que, apesar da minha proficiência em Linux, não irei abordar um tutorial de Linux nesse repositório, apenas algumas básicas explicações sobre o **porquê** eu estou configurando determinado arquivo ou modificando determinada linha.

<h3>
    <img src="https://github.com/Harlocks/design/blob/main/assets/inkscape/icons/apply.png?raw=true">
    Conteúdo
</h3>

[comment]: <> (Tabela de conteúdo)
<ul>
  <li><a href="#introducao"><img src="https://github.com/Harlocks/design/blob/main/assets/inkscape/icons/apply.png?raw=true"> <b>Introdução</b></a>
    <ul> <!-- Introdução -->
      <li><a href="#primeiros-passos">Primeiros Passos</a></li>
        <ul>
          <li><a href="#escolha-de-distribuicao">Escolha da distribuição</a></li>
          <li><a href="#criacao-de-usuario">Criação de usuário não <code>root</code></a></li>
          <li><a href="#configuracao-de-senha-forte">Configuração de uma senha forte</a></li>
          <li><a href="#atualizacao-do-sistema-base">Atualização do sistema base</a></li>
        </ul>
      <li><a href="#definindo-o-shell">Definindo o shell padrão</a></li>
      <li><a href="#removendo-o-motd">Varrendo o lixo para debaixo do tapete</a></li>
      <li><a href="#trocando-a-porta-do-ssh">Trocando a porta do SSH</a></li>
      <li><a href="#ativando-o-firewall">Ativando o Firewall</a></li>
    </ul>
  </li>
  <li><a href="#configurando-chaves"><img src="https://github.com/Harlocks/design/blob/main/assets/inkscape/icons/apply.png?raw=true"> <b>Configurando Chaves</b></a>
    <ul> <!-- Configurando Chaves -->
      <li><a href="#gerando-sua-chave-ssh">Gerando sua chave SSH</a></li>
      <li><a href="#gerenciando-chaves-ssh">Gerenciando chaves SSH</a></li>
      <li><a href="#configurando-autenticacao-de-chave-ssh">Configurando autenticação de chave SSH</a></li>
    </ul>
  </li>
  <li><a href="#configurando-autenticacao"><img src="https://github.com/Harlocks/design/blob/main/assets/inkscape/icons/apply.png?raw=true>"> <b>Configurando Autenticação</b></a>
    <ul> <!-- Configurando Autenticação -->
      <li><a href="#desabilitando-o-login-de-root">Desabilitando o login de <code>root</code></a></li>
      <li><a href="#utilizando-autenticacao-de-dois-fatores">Utilizando autenticação de dois fatores</a></li>
      <li><a href="#bloqueando-acessos-indevidos">Bloqueando acessos indevidos</a></li>
    </ul>
  </li>
  <li><a href="#gerenciando-servicos"><img src="https://github.com/Harlocks/design/blob/main/assets/inkscape/icons/apply.png?raw=true>"> <b>Gerenciando Serviços</b></a>
    <ul> <!-- Gerenciando Serviços -->
      <li><a href="#limitando-o-acesso-a-servicos">Limitando o acesso a serviços</a></li>
      <li><a href="#monitorando-e-registrando-acessos">Monitorando e registrando acessos</a></li>
      <li><a href="#configurando-logs-de-auditoria">Configurando logs de auditoria</a></li>
    </ul>
  </li>
  <li><a href="#atualizando-sistema"><img src="https://github.com/Harlocks/design/blob/main/assets/inkscape/icons/apply.png?raw=true>"> <b>Atualizando o Sistema</b></a>
    <ul> <!-- Atualizando o Sistema -->
      <li><a href="#habilitando-as-atualizacoes-automaticas">Habilitando as atualizações automáticas</a></li>
      <li><a href="#verificando-e-aplicando-patches-de-seguranca">Verificando e aplicando patches de segurança</a></li>
    </ul>
  </li>
</ul>