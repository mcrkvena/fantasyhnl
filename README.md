# FANTASY HNL
Aplikacija za slaganje vlastitog dream tima Hrvatske nogometne lige

Na temelju odabranih 11 igrača, računaju se pobjede, porazi i neriješeni ishodi te bodovi u svrhu uspoređivanja sa stvarnom tablicom

Ciljana publika: ljubitelji nogometa

# POSTAVLJANJE APLIKACIJE

1. otvorite command prompt (cmd.exe)
2. navigirajte do željenog direktorija (npr. "cd C:\Downloads")
3. upišite "git clone https://github.com/mcrkvena/fantasyhnl.git"
4. upišite "cd fantasyhnl"
5. ako imate instaliran yarn, upišite "yarn serve", ako ne, upišite "npm install" te "npm run serve" nakon instalacije
6. aplikaciji onda možete pristupiti putem localhosta na lokalnom serveru (http://localhost:8080/ ili http://localhost:8081/)

# KAKO APLIKACIJA FUNKCIONIRA

Registracija: Korisnik pri registraciji osim emaila i lozinke upisuje korisničko ime (koji se prikazuje pored tipke odjave) i naziv svog tima koji postaje naslov u kartici Moj Tim (team.vue). Ti se podaci također šalju u na bazu podataka u firebase.

Prijava: Korisnik mora upisati samo svoj email i lozinku.

Odabir igrača: Nakon registracije ili prijave, korisnik dolazi do kartice Moj Tim u kojoj iz 11 izbornika vrši izbor željenih igrača bez ikakvih ograničenja (osim nemogućnosti biranja istog igrača na dvije pozicije). Prilikom odabira, dolazi do promjene slike igrača UKOLIKO JE ONA DOSTUPNA. Nakon što korisnik odabere 11 igrača, postaje mu dostupna tipka Zaključaj Tim koja odabrane igrače šalje na bazu podataka u firebase. Pri ponovnom učitavanju stranice, ti se podaci povlače iz firebase-a te se automatski prikazuju.

Bodovanje: Svaki igrač ima 0, 1 ili 3 boda za svako kolo, ovisno o tome je li njegov tim pobjedio, izgubio ili remizirao. Računanje     bodova za korisnikov tim izvodi se na način da se uzme prosječni broj bodova svih 11 igrača za određeno kolo te na temelju rezultata korisnikovom se timu piše pobjeda (za prosječni proj bodova veći od 2.01), neriješeno (za prosječni broj bodova između 1.01 i 2.00) ili poraz (za prosječni broj bodova manji od 1.00)


Update 17.1.2020.: localStorage zamijenjen firebase firestore-om

Update 21.1.2020.: napravljen bodovni sustav

Update 28.1.2020.: uređen kod, dodane slike svih igrača, popravljene uočene greške
