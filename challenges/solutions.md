# Solutions

p1-b: tar -xvf challenges.tar.gz<br>
p2-b: cd challenges<br>
p3-b: ls challenges<br>
p4-b: mkdir foo<br>
p5-i: mkdir -r foo/bar/1/2/3<br>
p6-b: mkdir -r foo/bar/1/2/3<br>
p7-b: echo "Hello World"<br>
p8-b: echo "Hello World" >> hello.txt<br>
p9-b: touch empty.txt<br>
p10-b: rm -rf empty.txt<br>
p11-i: echo -n > empty.txt<br>
p12-i: cat > empty.txt<br>
p13-b: cp hello.txt goodbye.txt<br>
p14-b: mv goodbye.txt hello_copy.txt<br>
p15-i: cmp -s hello.txt hello_copy.txt && echo "identical" || echo "differents"<br>
p16-b: cat hello.txt hello_copy.txt > 2_hellos.txt<br>
p17-b: pwd<br>
p18-b: ls -l<br>
p19-b: echo "Some text to append" >> restricted.txt<br>
p20-b: ./hello_executable<br>
p21-b: chmod +x challenge_20 && ./challenge_20<br>
p22-b: gcc -o compile_me compile_me.c && ./compile_me<br>
p23-a: ./redirect > output.txt 2>&1<br>
p24-b: date<br>
p25-b: ps aux<br>
p26-b: nproc<br>
p27-b: uname -6<br>
p28-b: grep -rl "You found the needle in the haystack!" bunch_of_files/<br>
p29-b: head -n 25 people.csv<br>
p30-b: tail -n 25 people.csv<br>
p31-i: diff greeting1.txt greeting2.txt <br>
p32-i: echo "Hello" && sleep 5 && echo "world!"<br>
p33-i: dd if=/dev/zero of=zeros_file bs=1M count=1<br>
p34-i: dd if=/dev/urandom of=random_file bs=1M count=2<br>
p35-i: wc -l README.txt<br>
p36-b: tac README.txt<br>
p37-i: awk -F',' '{print $2}' people.csv<br>
p38-a: awk -F',' '{print $2}' people.csv | sort -u | wc -l<br>
p39-a: tail -n +2 people.csv | awk -F',' '{print $2}' | sort -u | wc -l<br>
p40-a: awk -F',' 'NR>1 {print $2}' people.csv | sort -u | wc -l<br>
p41-a: use "time" to compare<br>
p42-a: awk -F',' '$1=="Josiah" {count++} END {print count}' people.csv<br>
p43-i: find . -maxdepth 1 -type f | wc -l<br>
p44-i: find . -mindepth 1 -type d | wc -l<br>
p45-i: find . -type f -name "*deleteme*" -exec rm {} \;<br>
p46-i: grep -rl "You found the needle in the haystack!" bunch_of_files/ | xargs sed -i 's/You found the needle in the haystack!/The needle has been removed./g'<br>
p47-a: awk 'BEGIN {FS=","; OFS="|"} {$1=$1} 1' people.csv > people_pipe.csv<br>
p48-a: find bunch_of_files/ -type f -name "file001.rand" -exec cmp -s {} bunch_of_files/file001.rand \; -print<br>