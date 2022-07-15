# Grupo de estudos DS - Multicolinearidade no LGBM

Esse repositório contém o código utilizado para examinar os efeitos da colinearidade no LGBM. Muitos dizem que não precisamos remover variáveis com alta correlação do LGBM porque ele não é afetado. Isso somente é verdade se por "não afetado" quisermos dizer "capaz de ser estimado". O modelo sempre é estimado, mas isso não significa que ele não seja impactado pela colinearidade das variáveis.

O código nesse repositório mostra, com dados reais, os efeitos da colinearidade sobre o LGBM. Vemos que a colinearidade reduz significativamente a interpretabilidade do modelo, introduzindo viés no SHAP, sem acrescentar poder preditivo relevante. Se mantivermos variáveis redundantes no modelo (ou seja, muito correlacionadas), o modelo não saberá nos dizer o que foi importante na sua decisão. Ele dirá que cada variável sozinha é irrelevante, mas o conjunto é muito relevante. Ou seja, tudo é relevante e nada é relevante -- um paradoxo.
