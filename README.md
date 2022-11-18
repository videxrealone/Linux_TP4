# Linux_TP4 Les Processus
----
## Exercice 1 - Les processus, les signaux, premier plan et arrière plan

* **Quel est le numéro de processus (PID) de votre shell ?**

![image](https://user-images.githubusercontent.com/91763346/202722733-a94d2093-a499-48a9-8b89-36108420ff93.png)

* **Lancer en arrière plan (en terminant la commande par &) le programme gedit. Donner le PID et le PPID du processus ainsi lancé. Quel est son processus parent ? À quel terminal est-t-il rattaché ?**

![image](https://user-images.githubusercontent.com/91763346/202723964-a90372b2-4dc7-45a2-8421-4fb8c59079e3.png)

Le **PID** est **1963** et le **PPID** est **1257**. Il appartiant au terminal **kali** car le PPID est **1257** (Le meme PID que **kali**)

* **Utilisez la commande xclock -update 1 pour lancer une fenêtre “horloge”. Avez-vous le contrôle du terminal ?**

![image](https://user-images.githubusercontent.com/91763346/202724722-f5686179-d844-4647-a521-1eb8ac4fa6c9.png)

Pas de controle sur le terminal.

* **Tuez ce processus xclock.**

![image](https://user-images.githubusercontent.com/91763346/202724889-055a3351-684b-4c18-9480-194a088bb6c1.png)

* **Lancez-en un nouveau directement en arrière-plan. Pour cela, vous utiliserez le caractère & à la fin de la commande. La commande jobs vous permet d’obtenir la liste des processus en tâche de fond.**

![image](https://user-images.githubusercontent.com/91763346/202725454-88d50ae1-bd3b-418f-a09e-c89c00892bef.png)

![image](https://user-images.githubusercontent.com/91763346/202725590-1d86eb47-6e62-4860-bfec-0ca635862425.png)

* **Basculez le nouveau processus de xclock en avant-plan.**

![image](https://user-images.githubusercontent.com/91763346/202726157-e4b64f4e-8f3d-4137-b749-e624465041cb.png)

* **Suspendez le processus associé à xclock (vérifiez que l’horloge ne tourne pas.)**

![image](https://user-images.githubusercontent.com/91763346/202726926-87d865d9-2650-47b2-84ac-ee240afaf1a6.png)


* **Reprenez son exécution en arrière-plan (vérifiez que l’horloge a repris à tourner).**

![image](https://user-images.githubusercontent.com/91763346/202726746-d4f374f4-3d14-4f1e-951f-ed3f8223e30c.png)

![image](https://user-images.githubusercontent.com/91763346/202726511-cae9bac2-69f0-4c34-b44a-62c241e9337e.png)

* **Lancez un nouveau terminal. Dans ce nouveau terminal listez tous les processus qui vous appartiennent.**

![image](https://user-images.githubusercontent.com/91763346/202727254-89ad2c97-4caa-4637-8595-b4d19a4b0662.png)

* **Visualiser la liste des signaux du système avec la commande kill -l**

![image](https://user-images.githubusercontent.com/91763346/202727427-b5ecf02c-e6f0-4184-9236-155bcaccf91f.png)

* **Mettez un suspension le processus de xclock en utilisant la commande kill (vérifiez que l’horloge ne tourne pas).**

![image](https://user-images.githubusercontent.com/91763346/202728389-551c206b-7c38-4682-96ed-fe0b219e9b3c.png)


![image](https://user-images.githubusercontent.com/91763346/202728170-3392938e-4a47-4cc9-a05d-6c6f181bbbf0.png)

![image](https://user-images.githubusercontent.com/91763346/202728643-acf332f8-32c7-435e-b553-3b0082f8fc04.png)

* **Reprenez l’exécution de xclock en utilisant la commande kill (vérifiez que l’horloge a repris à tourner).**

![image](https://user-images.githubusercontent.com/91763346/202729366-b4fac7ed-caa5-4aa8-a5f1-7dcd205c084e.png)

* **Tuez xclock avec la commande kill.**

![image](https://user-images.githubusercontent.com/91763346/202729716-f330161e-5c71-4a44-85ca-8ccc5c6bcfa7.png)

## Exercice 2 - Les commandes nice et renice : Manipulation des priorités

* **Créer le processus sleep 500 en arrière plan en lui affectant la priorité 15**

![image](https://user-images.githubusercontent.com/91763346/202730820-043ccae7-8211-4734-9888-aa66899bdb15.png)

* **Modifier la priorité du processus sleep 500 à 18**

![image](https://user-images.githubusercontent.com/91763346/202732774-8e3b7a5e-6eb7-4e82-bfa0-dc639a672dc0.png)

* **Sans passer en mode superuser, essayer de modifier la priorité du processus sleep 500 à -5. Est-ce que c’est possible ?
Non on ne peut que diminuer la priorité (doit etre <18 dans notre cas).**


* **Passer en mode superuser (en utilisant sudo) et modifier la priorité du processus sleep 500 à -5.**

![image](https://user-images.githubusercontent.com/91763346/202733544-94ad03b0-a2c5-4655-8bf0-a86cc3af0501.png)

* **Lancer un processus sleep 1200 en arrière plan en lui affectant la priorité -10.**

![image](https://user-images.githubusercontent.com/91763346/202734313-dd23f477-78fa-45a0-a738-9e421ccafa63.png)

