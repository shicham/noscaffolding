# noscaffolding

**Astuce du bloc d'initialisation Java**

astuce intéressante que Kevlin Henney a trouvée dans du code que Michael Feathers a publié sur [http://pastie.org/534364](http://pastie.org/534364). Au lieu de faire ceci :

ArrayList<Integer> values = new ArrayList<Integer>();<br/>;
values.add(1);<br/>;
values.add(2);<br/>;
values.add(3);<br/>;

Tu peux le faire:
ArrayList<Integer> values = new ArrayList<Integer>() {{<br/>;
    add(1);<br/>;
    add(2);<br/>;
    add(3);<br/>;
}};

