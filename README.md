# Linux
# Script NAC 

#!/bin/bash

# Menu Shell


SCRIPT=`basename $0`
LOG=`echo /var/log/scripts/$SCRIPT | sed s/'.sh'/'.log'/g`
LOG=/var/log/arquivo.log
exec 1>>${LOG}
exec 2>&1
echo "[`date`] ==== Inicio de rotina"
comando_com_output01

menu ()
{
a="ok"

while true $a !="ok"
do
   echo "MENU PRINCIPAL"
   echo ""
   echo "1 - Adicionar um usuário echo "add usuario: "
	read usuario
	adduser $usuario"
    echo "senha do usuario $usuario: "
	passwd $usuario"

   echo "2 - Adicionar usuário ao Grupo echo "add grupo: "
	read grupo
	addgroup $grupo"

   echo "3 - Alterar a senha de um usuário echo -e "new_password\nnew_password" | (smbpasswd -a -s $usuario)"

   echo "4 - Remover usuário echo "del usuario: "
	read usuario
	deluser $usuario "

   echo "5 - Remover grupo echo "del grupo: "
	read grupo
	delgroup $grupo"
	
   echo "6

   echo "Digite a opção desejada: "
   read a
   case $a in

	

   esac
done
}

comando_com_output02
echo "[`date`] ==== Fim de rotina"


