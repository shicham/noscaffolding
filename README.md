# noscaffolding

Astuce du bloc d'initialisation Java

astuce intéressante que Kevlin Henney a trouvée dans du code que Michael Feathers a publié sur http://pastie.org/534364. Au lieu de faire ceci :

ArrayList<Integer> values = new ArrayList<Integer>();\n
values.add(1);
values.add(2);
values.add(3);

Tu peux le faire:

ArrayList<Integer> values = new ArrayList<Integer>() {{
    add(1);
    add(2);
    add(3);
}};
