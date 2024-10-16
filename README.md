# Scripts
Por que esse repositório existe? Bom, deste de que eu resolvi trocar o `Windows` pelo o `Ubuntu` não vejo motivos para voltar para o `Windows`. E como estou "surgando a onda" de criar _scripts_ personalizados, resolvi armazená-los para quando eu precisar formatar ou algo do tipo (já aconteceu).

## Lista

- `cleanup`:
    - *O que faz?* Não se engane pelo nome, esse script apenas move o conteúdo da área de `_swap_` para a memória `RAM`;
    - *Contexto?* Quando eu abro muitos aplicativos e loto a memória `RAM`, o `Ubuntu` assim como em muitos sistemas operacionais, começa a armazenar parte dos processos na área de `_swap_`, que fica na memória secundária (disco, ssd, etc) e leva muito tempo para ser acessado. Claro que fechar os aplicativos (parando os processos deles) libera o espaço ocupado pelo processo tanto na `RAM` como na área de `_swap_`. Porém, eu percebi que nesses casos de lotação de memória as vezes o `Ubuntu` jogava também para a `_swap_` processos dele próprio, e quando eu encerrava os outros ele não trazia o conteúdo desses processos importantes dele de volta para a `RAM`, ocasionando travamentos. Não sei se na verdade ele faz isso depois de um tempo X, mas esse script faz isso em pouco tempo desativando a área de `_swap_` e ativando novamente (ela é importante também).