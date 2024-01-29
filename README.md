# WECHALL STD23042 :seedling:

Pour commencer le challenge, il faut se connecter sur votre compte ssh: sssh -p 19198 user@warchaal.net
Nous allons utiliser ces commande:

- **cd**: changer la direction

- **ls -a**: affichier le contenu

- **cat**: pour lire un fichier 

- **chmod +r**: pour avoir la permiission de lire

## Level 0
```bash
cd /home/level
ls -a
cd 00-welcom
ls -a
cat README.md
```

## Level 1
```bash
cd /home/level
ls -a
cd -choise tree
ls -a
cd blue
cd hats
cd grey
cat solution.txt
```

## Level 2
```bash
cd /home/level
ls -a
cd 02
ls -a
cd .prob
ls -a
cat solution
```

## Level 4
```bash
cd /home/user/username/level
ls -a
cd 04-kwisat
ls -a
chmod +r README.md
cat README.md
```

## Level 5
```bash
cd /home/level
ls -a
cd 05-privacy
ls -a
cat README.md
```
## Pytong

- **step1**: Create a file in our directory (ex: `uwu.txt`)

- **step2**: Create a scripts or code which can change to content of `uwu.txt` every X time

- I do it just with bash

```bash
#!/bin/bash

end_time=$((SECONDS+15))

while [ $SECONDS -lt $end_time ]; do
    echo "d" >> uwu.txt
    sleep 0.0005
done
```

The scritps just add the letter `d` in the `uwu.txt` every `0.0005`( you can adjust it's values)
The end_time is optional

- **step3**: Connect to wechall with another terminal and go to the pytong folder ( `/home/level/12_pytong`) 

- **step4**: Go back to the other terminal and run your scripts (which add `d` in `uwu.txt` here) 

- **step5**: Now go back to your pytong terminal and run the following command (just make sure to do this before the end_time of your scripts is achieved) 

```bash
./pytong ~/uwu.txt
```
That's it

## Tryouts
How ? : Quite easy, tryouts use `cat` command which the path is not specify, so we need just to create a fake cat command

- **step1**: Here is an example of cat command ( put it in your home directory for example)

```c
//Colleo eto ilay code C nalefako iny
```

- **step2**: Create a file in your home directory called `seed` ('cause it's required by tryouts)

- **step3**: Add your home directory to PATH
```bash
export PATH=$HOME:$PATH
```

- **step4**: run the tryouts executable in it's folder

- **step5**: That's it, open new terminal and just use `cat` to read the file seed, and the solution will apear 

