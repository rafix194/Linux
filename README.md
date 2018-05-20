# Linux
# Script NAC 

#!/bin/bash

# Menu Shell

menu ()
{
a="ok"

while true $a !="ok"
do
   echo "MENU PRINCIPAL"
   echo ""
   echo "1- echo "add usuario: "
	read usuario
	adduser $usuario"

   echo " 2- echo "senha do usuario $usuario: "
	passwd $usuario"

   echo "3 - echo "add grupo: "
	read grupo
	addgroup $grupo"

   echo "4 - echo -e "new_password\nnew_password" | (smbpasswd -a -s $usuario)"

   echo "5 - echo "del usuario: "
	read usuario
	deluser $usuario "

   echo "6 - echo "del grupo: "
	read grupo
	delgroup $grupo"

   echo "Digite a opção desejada: "
   read a
   case $a in

	

   esac
done
}

$ git tag
v1.0
