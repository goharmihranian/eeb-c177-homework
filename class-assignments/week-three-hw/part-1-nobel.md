1) 

CHemistry: 181
cut -d "," -f 3 nobel.csv | grep -w chemistry | wc

Economics: 81
cut -d "," -f 3 nobel.csv | grep -w economics | wc

Literature: 114
cut -d "," -f 3 nobel.csv | grep -w literature | wc

Medicine: 216
cut -d "," -f 3 nobel.csv | grep -w medicine | wc

Peace: 133
cut -d "," -f 3 nobel.csv | grep -w peace | wc

Physics: 210
cut -d "," -f 3 nobel.csv | grep -w physics | wc

2)
cut -d "," -f 5-6 nobel.csv | sort | uniq -d
"Comité international de la Croix Rouge (International Committee of the Red Cross)",NA
"Frederick","Sanger"
"John","Bardeen"
"Linus Carl","Pauling"
"Marie","Curie
"Office of the United Nations High Commissioner for Refugees (UNHCR)",NA

3) 
cut -d "," -f 6 nobel.csv | sort | uniq -d
Wilson
Fischer
Lewis
Muller
Lee
Smith

4) cut -d "," -f 3 nobel.csv | grep -w -E 'chemistry|medicine|economics|literature|peace|physics' | sort | uniq -c
output:
    181 "chemistry"
     81 "economics"
    114 "literature"
    216 "medicine"
    133 "peace"
    210 "physics"
medicine won highest number, economics won lowest


