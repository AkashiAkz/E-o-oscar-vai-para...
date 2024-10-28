Quantos Oscars Natalie Portman ganhou?
R: 1 
Q: SELECT count(*) FROM indicados_ao_oscar WHERE nome_do_indicado Like "%Natalie Portman%" and vencedor = "true";
 
Amy Adams já ganhou algum Oscar?
R: Não
Q: SELECT * FROM indicados_ao_oscar WHERE nome_do_indicado Like "%Amy Adams%";
 
A série de filmes Toy Story ganhou um Oscar em quais anos?
R: Anos vencedores foram: 2011 (sendo dois filmes vencedores) 2020 (um oscar vencedor)
Q: SELECT * FROM indicados_ao_oscar WHERE nome_do_filme Like "%Toy Story%" and vencedor = "true";
 
A partir de que ano que a categoria "Actress" deixa de existir?
R: A partir de 1976
Q: SELECT * FROM indicados_ao_oscar WHERE categoria = "Actress";
 
Quem ganhou o primeiro Oscar para Melhor Atriz? Em que ano?
R: Foi no ano de 1928
Q: SELECT * FROM indicados_ao_oscar WHERE categoria Like "%Actress%" and vencedor = "true";
 
Na campo "Vencedor", altere todos os valores com "true" para 1 e todos os valores "false" para 0.
Q: para true: 
            update indicados_ao_oscar
            set  vencedor = "1"
            where vencedor = "true";
para false: 
            update indicados_ao_oscar
            set  vencedor = "0"
            where vencedor = "false";
 
Em qual edição do Oscar "Crash" concorreu ao Oscar?
R: Edição de 2006
Q: select * from indicados_ao_oscar where nome_do_filme = "Crash";
 
O filme Central do Brasil aparece no Oscar?
R: Sim
Q: select * from indicados_ao_oscar where nome_do_filme = "Central Station";
 
Inclua no banco 3 filmes que nunca foram nem nomeados ao Oscar, mas que merecem ser.
R: INSERT INTO indicados_ao_oscar(ano_filmagem,ano_cerimonia,cerimonia,categoria,nome_do_indicado,nome_do_filme,vencedor) VALUES (2010,2011,96,'ACTOR IN A LEADING ROLE','Michael Cera.','comedy','true');
INSERT INTO indicados_ao_oscar(ano_filmagem,ano_cerimonia,cerimonia,categoria,nome_do_indicado,nome_do_filme,vencedor) VALUES (2013,2014,96,'ACTRESS IN A LEADING ROLE','Rachel McAdams','Sci-Fi','true');
INSERT INTO indicados_ao_oscar(ano_filmagem,ano_cerimonia,cerimonia,categoria,nome_do_indicado,nome_do_filme,vencedor) VALUES (1995,1996,96,'ANIMATED FEATURE FILM','Hideaki Anno','Sci-fi','true');
 
Denzel Washington já ganhou algum Oscar?
R: Ja ganhou sim, 2 Oscars
Q: select * from indicados_ao_oscar where nome_do_indicado like "%Denzel Washington%" and vencedor = "true";
 
Quais os filmes que ganharam o Oscar de Melhor Filme?
R: A Beautiful Mind
A Man for All Seasons
Amadeus
American Beauty
Annie Hall
Argo
Birdman or (The Unexpected Virtue of Ignorance)
Braveheart
Chariots of Fire
Chicago
CODA
Crash
Dances With Wolves
Driving Miss Daisy
Everything Everywhere All at Once
Forrest Gump
Gandhi
Gladiator
Green Book
In the Heat of the Night
Kramer vs. Kramer
Lawrence of Arabia
Midnight Cowboy
Million Dollar Baby
Moonlight
My Fair Lady
No Country for Old Men
Nomadland
Oliver!
One Flew over the Cuckoo's Nest
Oppenheimer
Ordinary People
Out of Africa
Parasite
Patton
Platoon
Rain Man
Rocky
Schindler's List
Shakespeare in Love
Slumdog Millionaire
Spotlight
Terms of Endearment
The Artist
The Deer Hunter
The Departed
The English Patient
The French Connection
The Godfather
The Godfather Part II
The Hurt Locker
The King's Speech
The Last Emperor
The Lord of the Rings: The Return of the King
The Shape of Water
The Silence of the Lambs
The Sound of Music
The Sting
Titanic
Tom Jones
Unforgiven
Q: select * from indicados_ao_oscar where categoria like "%BEST PICTURE%" and vencedor = "true";
 
Bonus: Quais os filmes que ganharam o Oscar de Melhor Filme e Melhor Diretor na mesma cerimonia?
 
Bonus: Denzel Washington e Jamie Foxx já concorreram ao Oscar no mesmo ano?
