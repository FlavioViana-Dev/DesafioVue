# Vue Coding Challenge - Batalha de Monstros

## Introdução

Você criará um vídeo de gravação de tela de si mesmo concluindo o desafio e me enviará um link para o arquivo via Google Drive. Algumas coisas a considerar:

- Pedimos que conclua este desafio dentro do prazo acordado em nossa conversa.
- **NÃO DEVE editar seu vídeo, interrompê-lo e continuar depois, usar uma segunda tela, copiar conteúdo de telas ocultas ou qualquer coisa semelhante que possa ser considerada trapaça. A gravação deve ser sem interrupção e sem edição.**
- **Você DEVE mostrar o relógio do seu sistema operacional durante toda a gravação. Por favor, não maximize sua tela de forma que o relógio do sistema operacional fique oculto. Mantenha-o sempre visível.**
- Você pode usar um software de gravação de tela como Loom, QuickTime ou algo semelhante para criar o vídeo.
- A gravação deve ser de todo o desafio de codificação, do começo ao fim, que tem cerca de 70 minutos.
    - **Você usará 45 minutos para o desafio de codificação e 25 minutos para o desafio de resolução de problemas.**
    - Lembre-se de gravar o desafio de codificação e o desafio de resolução de problemas **juntos em apenas um vídeo**; por favor **não pare/reproduza e entre no vídeo**; se o fizer, será desqualificado.
    - Você pode gastar mais de 45 minutos no desafio de codificação, mas iremos descontar pontos no seu desafio. Mas, por favor, tenha cuidado com o limite de 25 minutos no desafio de resolução de problemas; você deve evitar gastar mais do que o limite de tempo.
- Você deve gravar toda a sua tela para que possamos validar sua implementação corretamente. **Além disso, o relógio do seu computador deve estar visível em todo o vídeo.**
- Envie o arquivo de vídeo para o Google Drive e compartilhe um link aberto conosco (suportamos .mp4, arquivos menores/com menos de 4 GB).
- Ao concluir o desafio, explique o que está fazendo. Acompanhe-nos através de seu pensamento, explique suas decisões, etc. Mostre-nos seu trabalho de interface do usuário, se aplicável.

## O desafio de codificação

### Começando

Oi! Bem-vindo ao desafio de codificação Vue.js! Queremos verificar seu conhecimento de Vue.js dando a você um aplicativo para terminar. Já temos um requerimento, mas está incompleto; seu objetivo é concluir este aplicativo e torná-lo utilizável.

> *Temos um projeto estruturado com um padrão, então o tempo sugerido acima pode ser feito seguindo o padrão e dividindo seu tempo em categorias; uma boa organização o levará a terminar o desafio com sucesso!*
>

> *Lembre-se de que não estamos solicitando que você crie um aplicativo responsivo; você pode se concentrar apenas na versão web.*
>

<à parte>
⏳ **Duração recomendada para cada categoria do desafio (essa é uma sugestão)
  -** **Estilização**: 15 minutos
  **- Criação de componentes**: 10 minutos
  **- Lojas e ajudantes**: 10 minutos
  **- Teste de unidade**: 10 minutos

*Claro, você pode dividir o tempo como quiser, mas recomendamos que você siga isso.*

</aside>

### Instruções

O aplicativo atual exibe uma lista de monstros. No momento, temos apenas o recurso de selecionar os monstros do jogador; seu trabalho é implementar as funcionalidades que faltam.

Você terá que criar o componente da carta do monstro para que possamos visualizar corretamente os pontos fortes e fracos do monstro.

Após selecionar o monstro do jogador, você terá que implementar a lógica para pegar o monstro do computador, que deverá ser selecionado aleatoriamente, não permitindo ser o mesmo selecionado do jogador; lembre-se que você irá selecionar o monstro do jogador clicando nele.

Uma vez selecionados os dois monstros, o usuário pode “iniciar a batalha” e você deve implementar a solicitação de serviço. Já temos um endpoint pronto para isso. Você não precisa se preocupar com a implementação do endpoint ou mesmo com a lógica para calcular o batalha do monstro; seu trabalho será fazer a solicitação e exibir o resultado da batalha corretamente.


###API

Temos nossa API local configurada dentro do projeto. Para iniciá-lo, você deve executar o comando `npm run serve:data`, que iniciará o servidor.

*Não recomendamos que você altere nenhum dado dentro da pasta `data`; seu objetivo é implementar o desafio com os dados já fornecidos e em execução.*

Temos dois endpoints, que são os seguintes:

- `GET /monsters`: Este endpoint retornará todas as informações necessárias para a lista de monstros.
- `POST /battle`: Este endpoint receberá um corpo e retornará o resultado da batalha.

O `GET /monsters` retorna o seguinte contrato quando solicitado:

```bash
[
{
"Eu fiz",
"nome": "Monstro 1",
"ataque": 20,
"defesa": 30,
"cv": 100,
"velocidade": 50,
"tipo": "Tipo",
"imageUrl": "url"
}
]
```

O `POST /battle` espera receber um corpo com as informações dos monstros; o corpo esperado é o seguinte:

```bash
{
"monstro1Id": "monstro-1",
"monstro2Id": "monstro-2"
}
```

### Tecnologias

Este projeto é construído usando as bibliotecas do ecossistema Vue.js; é bom você conhecer os seguintes itens para ter um bom desempenho:

- [Typescript](https://www.typescriptlang.org/docs/)
- [Vue.js](https://v2.vuejs.org/v2/guide/)
- [Vuex](https://vuex.vuejs.org/)
- [Vuetify](https://vuetifyjs.com/en/)
- [Jest](https://jestjs.io/docs/getting-started)
- [Utilitários de teste Vue](https://v1.test-utils.vuejs.org/guides/#getting-started)

### Critérios de Aceitação

1. A implementação corresponde ao design
2. Os testes são aprovados e a cobertura foi adicionada para cobrir as mudanças e novas implementações
3. O monstro do computador é selecionado aleatoriamente após selecionar o monstro do jogador
4. A mensagem do vencedor deverá ser apresentada após a batalha


## O desafio de resolução de problemas

Oi! Bem-vindo ao desafio do código de solução de problemas do TypeScript; queremos testar suas habilidades de resolução de problemas aqui.

Você receberá um repositório com alguns desafios e terá que resolvê-los implementando e fazendo passar todos os testes criados.

> Por favor, lembre-se de **NÃO USAR O GOOGLE** para resolver os desafios de raciocínio; tente resolvê-los sozinho.
>

### Desafios

Forneceremos três desafios no repositório; você terá um limite de tempo mencionado acima minutos para resolvê-los e fazê-los passar nos testes.

*Caso não consiga terminar todos os desafios, envie o registro com o que você resolveu, que iremos avaliar.*

Lembre-se de resolvê-los usando TypeScript puro, e evite usar bibliotecas ou qualquer coisa que não seja seu código; queremos ver você pensando e resolvendo o desafio.

Você pode fazê-los em qualquer ordem, mas lembre-se de que alguns desafios são mais complexos do que outros.

**Ao final do desafio, faça os testes para nós antes de parar a gravação. Esta etapa é crítica; se você esquecer de fazê-lo, isso causará sua desqualificação.**

### Critérios de Aceitação

1. O código deve ser legível.
2. O código deve ser fácil de manter.
3. O código não deve ser complexo.
4. Todos os testes devem passar.
5. **Testes aprovados**
