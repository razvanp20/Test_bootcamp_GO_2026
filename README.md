# Test_bootcamp_GO_2026

Problema practica Bootcamp 2026	

Aveți în față un schelet de aplicație numit BookShop care e compus dintr-un server http scris în GO si o baza de date PostgreSQL. Pornind de la acesta, rezolvați următoarele cerințe: 
1. Este conexiunea la baza de date funcțională? Daca nu, reparati-o din docker-compose.
2. Modificați codul aplicației astfel incat endpointul POST /books să fie funcțional
3. Creați modelul și tabela pentru obiecte de tip Publisher care sa contina urmatoarele campuri: name, phone number si email. 
    1. Adaugati o relatie one to many intre entitatea Publisher și entitatea Book.
    2. Adaugati endpointuri http pe calea “/publishers” de tip POST si DELETE.
        1. Ce se intampla cand o carte ramane fara editura? Ce constrângere puteți pune pe relația editura-carte?
    3. Scrieti un endpoint HTTP GET /book/{id}. Aveți grija ca detaliile editurii sa fie incluse.
4. Scrieti un endpoint HTTP GET /books care suporta urmatorii query params:
    1. An publicare (doar relație de egalitate)
    2. Nume editura (doar relație de egalitate)
5. Scrieți o funcție care rulează “în background”, in paralel cu rutina principala. Aceasta functie va număra cate requesturi au fost făcute de la începutul programului și va scrie acest număr la fiecare 5 secunde în fișierul “statistics.out”.
