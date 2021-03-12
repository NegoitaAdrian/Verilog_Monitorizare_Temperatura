# Verilog_Monitorizare_Temperatura
Implementați în Verilog un circuit combinațional care are ca scop simularea monitorizării în cadrul unei
sere și afișarea ei într-o formă vizuală (ieșire scalată cu afișaj de tip LED). Circuitul va extrage de fiecare
dată temperaturile senzorilor activi, va efectua media lor aritmetică și va afișa temperatura aproximată întro manieră codată, pretabilă ca semnal de activare pentru fiecare bec de tip LED, emițând o alarmă în cazul
în care temperatura este în afara valorilor admise.
Valorile de intrare ale tuturor senzorilor sunt reprezentate pe 8 biți și sunt concatenate într-un vector de biți,
astfel: [7:0] - valoarea primului senzor, [15:8] - valoarea celui de-al doilea senzor, etc. Fiecare senzor are
un bit de enable care marchează faptul că valoarea trimisă de senzor este validă și poate fi citită.
Ieșirea modulului va fi aproximată la întregul cel mai apropiat și poate fi reprezentată doar în intervalul
[19:26], orice valoare în afara acestui interval activând un semnal de alarmă. Aceasta este codificată întrun mod scară
