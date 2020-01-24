1)
EX: 29
cut -d "," -f 10 European_Red_List.csv | grep -w EX | wc

RE: 8
cut -d "," -f 10 European_Red_List.csv | grep -w RE | wc

CR: 472
cut -d "," -f 10 European_Red_List.csv | grep -w CR | wc

EN: 687
cut -d "," -f 10 European_Red_List.csv | grep -w EN | wc

VU: 885
cut -d "," -f 10 European_Red_List.csv | grep -w VU | wc

NT: 964
cut -d "," -f 10 European_Red_List.csv | grep -w NT | wc

LC: 5805
cut -d "," -f 10 European_Red_List.csv | grep -w LC | wc

DD: 2409
cut -d "," -f 10 European_Red_List.csv | grep -w DD | wc

NA: 411
cut -d "," -f 10 European_Red_List.csv | grep -w NA | wc

2)

EX: 2
cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w EX | sort | uniq -c | wc

RE: 4
cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w RE | uniq -c | wc

CR: 10
cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w CR | sort | uniq -c | wc

EN: 18
cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w EN | sort | uniq -c | wc

VU: 39
cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w VU | sort | uniq -c | wc

NT: 32
cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w NT | sort | uniq -c | wc

LC: 428
cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w LC | sort | uniq -c | wc

DD: 0
cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w DD | sort | uniq -c | wc

NA: 0
 cut -d "," -f 4-10 European_Red_List.csv | grep -w AVES | grep -w NA | sort | uniq -c | wc

3)
cut -d "," -f 4,5,10 European_Red_List.csv | grep -w AVES | grep -E 'EX|RE|CR' | grep -v -E 'EN|VU|NT|LC|DD|NA' | sort | uniq -c
output:
1 AVES,ACCIPITRIFORMES,CR
      3 AVES,CHARADRIIFORMES,CR
      2 AVES,CHARADRIIFORMES,EX
      1 AVES,CHARADRIIFORMES,RE
      1 AVES,OTIDIFORMES,CR
      3 AVES,PASSERIFORMES,CR
      1 AVES,PASSERIFORMES,RE
      1 AVES,PELECANIFORMES,RE
      1 AVES,PROCELLARIIFORMES,CR
      1 AVES,STRIGIFORMES,CR
      1 AVES,SULIFORMES,RE


