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
p15-i: cmp -s hello.txt hello_copy.txt && echo "identical" || echo "differents"