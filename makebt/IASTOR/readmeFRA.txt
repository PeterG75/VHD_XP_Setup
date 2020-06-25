﻿************************************************************
************************************************************
* Fichier Readme pour l'installation d'Intel(R) Matrix 
* Storage Manager.
*
* Reportez-vous à la configuration requise pour une liste
* des systèmes d'exploitation pris en charge par Intel(R) 
* Matrix Storage Manager.
*
* Ce document contient des références à des produits
* développés par Intel. Certaines restrictions
* d'utilisation de ces produits existent, de même que des
* restrictions de divulgation des informations à des tiers. 
* Veuillez lire la section Avis de non-responsabilité au
* bas de ce document et contactez votre représentant Intel
* si vous souhaitez obtenir des informations supplémentaires.
*
************************************************************
************************************************************

************************************************************
* Intel n'émet aucune déclaration de facilité d'utilisation, 
* d'efficacité ou de garantie. Le CONTRAT DE LICENCE DU 
* LOGICIEL INTEL contenu dans ce document définit, de façon 
* complète, la licence et l'utilisation de ce logiciel.
************************************************************


************************************************************
* CONTENU DE CE DOCUMENT
************************************************************

Ce document contient les sections suivantes :

1.  Présentation
2.  Configuration requise
3.  Langues prises en charge
4.  Détermination du mode système
5.  Installation du logiciel
6.  Vérification de l'installation du logiciel
7.  Instructions d'installation avancées
8.  Identification du numéro de version du logiciel
9.  Désinstallation du logiciel
10. Ouverture de l'interface utilisateur Option ROM
11. Gestion des volumes RAID dans l'Option ROM
12. Options de réinitialisation du volume RAID dans 
    l'Option ROM
13. Vérification de la version du logiciel Option ROM


************************************************************
* 1.  PRÉSENTATION
************************************************************

Intel(R) Matrix Storage Manager est conçu pour fournir
une fonctionnalité aux contrôleurs de stockage suivants :
    Contrôleurs RAID :
    - Intel(R) ICH8M-E/ICH9M-E SATA RAID Controller    
    - Intel(R) ICH8R/ICH9R/ICH10R/DO SATA RAID Controller   
    - Intel(R) ESB2 SATA RAID Controller  
    - Intel(R) ICH7MDH SATA RAID Controller
    - Intel(R) ICH7R/DH SATA RAID Controller  

    Contrôleurs AHCI :
    - Intel(R) ICH10D/DO SATA AHCI Controller 
    - Intel(R) ICH10R SATA AHCI Controller
    - Intel(R) EP80579 SATA AHCI Controller
    - Intel(R) ICH9M-E/M SATA AHCI Controller
    - Intel(R) ICH9R/DO/DH SATA AHCI Controller
    - Intel(R) ICH8M-E/M SATA AHCI Controller
    - Intel(R) ICH8R/DH/DO SATA AHCI Controller
    - Intel(R) ESB2 SATA AHCI Controller
    - Intel(R) ICH7M/MDH SATA AHCI Controller
    - Intel(R) ICH7R/DH SATA AHCI Controller   


************************************************************
* 2.  CONFIGURATION REQUISE
************************************************************

1.  Le système doit contenir un processeur Intel(R) Core(TM)2 
    Duo ou Intel(R) Core(TM)2 Extreme ou Intel(R) Pentium(R) 
    Processor ou Intel(R) Xeon(R) Processor et un des
    produits Intel compris dans la section 1 ci-dessus.


2.  Le système doit exécuter un des systèmes d'exploitation
    suivants :
    - Microsoft* Vista*
    - Microsoft* Vista* x64 Edition (REMPARQUE 1)    
    - Microsoft* Windows* Server 2008
    - Microsoft* Windows* Server 2008 x64 Edition (REMARQUE 1)
    - Microsoft* Windows* XP Home Edition
    - Microsoft* Windows* XP Professional
    - Microsoft* Windows* XP x64 Edition (REMPARQUE 1)
    - Microsoft* Windows* Server 2003
    - Microsoft* Windows* Server 2003, 
      Web x64 Edition (REMARQUE 1)
    - Microsoft* Windows* Server 2003, 
      Standard x64 Edition (REMARQUE 1)
    - Microsoft* Windows* Server 2003, 
      Enterprise x64 Edition (REMARQUE 1)
    - Microsoft* Windows* Media Center Edition

REMARQUE 1 : Si le système exécute une version Windows 64 bits,
	     le pilote Intel(R) Matrix Storage Manager prenant 
	     en charge 64 bits doit être utilisé.

3.  Les systèmes d'exploitation suivants ne sont pas pris 
    en charge :

    Toute version des systèmes d'exploitation Microsoft suivants :
    - MS-DOS
    - Windows 3.1
    - Windows NT 3.51
    - Windows 95
    - Windows 98
    - Windows Millennium Edition (Me)
    - Windows NT 4.0
    - Windows 2000 Datacenter Server
    - Windows 2000 Professional
    - Windows 2000 Advanced Server

    Toute version des systèmes d'exploitation suivants :
    - Linux
    - UNIX
    - BeOS
    - MacOS
    - OS/2

4.  Le système doit contenir au minimum la mémoire système
    requise par le système d'exploitation.

5.  L'Utilitaire d'installation du logiciel pour les jeux de 
    composants Intel(R) doit être installé avant d'installer
    Intel(R) Matrix Storage Manager.


************************************************************
* 3.  LANGUES PRISES EN CHARGE
************************************************************

Vous trouverez ci-dessous la liste des langues (et leur 
abréviation) disponibles pour le logiciel Intel(R) Matrix 
Storage Manager. Le code de langue est affiché entre 
parenthèses après chaque langue.

ARA -> Arabe (Arabie saoudite) 	(0401)
CHS -> Chinois (simplifié) 	(0804)
CHT -> Chinois (traditionnel)	(0404)
CSY -> Tchèque 			(0405)
DAN -> Danois 			(0406)
NLD -> Néerlandais 		(0413)
ENU -> Anglais (États-Unis) 	(0409)
FIN -> Finnois 			(040B)
FRA -> Français (international) (040C)
DEU -> Allemand 		(0407)
ELL -> Grec 			(0408)
HEB -> Hébreu 			(040D)
HUN -> Hongrois 		(040E)
ITA -> Italien			(0410)
JPN -> Japonais 		(0411)
KOR -> Coréen 			(0412)
NOR -> Norvégien 		(0414)
PLK -> Polonais 		(0415)
PTB -> Portugais (Brésil) 	(0416)
PTG -> Portugais (standard) 	(0816)
RUS -> Russe 			(0419)
ESP -> Espagnol 		(040A)
SVE -> Suédois 			(041D)
THA -> Thaï 			(041E)
TRK -> Turc 			(041F)


************************************************************
* 4.  DÉTERMINATION DU MODE SYSTÈME
************************************************************

Pour utiliser ce fichier Readme efficacement, vous devez
déterminer le mode de votre système. Le moyen le plus facile
de déterminer le mode consiste à identifier la façon dont le
contrôleur est présenté dans le Gestionnaire de périphériques.
La procédure suivante vous guidera pas à pas afin de 
déterminer le mode.

1.  Dans le menu Démarrer :
    1a. Sous Windows* Vista ou les systèmes d'exploitation 
        ultérieurs, sélectionnez Panneau de configuration.

2.  Ouvrez l'applet "Système" (vous devrez peut-être 
    d'abord sélectionner "Basculer vers l'affichage 
    classique").

3.  Sélectionnez l'onglet "Matériel". 

4.  Sélectionnez le bouton "Gestionnaire de périphériques".

5.  Dans le Gestionnaire de périphériques, recherchez une
    entrée intitulée "Contrôleurs de stockage" sous Windows  
    Vista et "Contrôleurs SCSI et RAID" sous Windows XP et 
    des systèmes d'exploitation ultérieurs. Si cette entrée  
    existe, développez-la et recherchez un des contrôleurs
    figurant dans la présentation (section 1). Si le contrôleur
    identifié est un contrôleur RAID, alors le système est en
    mode RAID.
 
    Si aucun des contrôleurs ci-dessus n'est affiché,
    le système n'est pas en mode RAID et vous devez
    passer à l'étape 6 ci-dessous.

6.  Dans le Gestionnaire de périphériques, recherchez une
    entrée "Contrôleurs IDE ATA/ATAPI". Si cette entrée  
    existe, développez-la et recherchez un des contrôleurs
    figurant dans la présentation (section 1). Si le contrôleur
    identifié est un contrôleur AHCI, alors le système est en
    mode AHCI.

    Si aucun des contrôleurs ci-dessus n'est affiché,
    le système n'est pas en mode AHCI. Aucun autre mode
    n'est pris en charge par le logiciel Intel(R) Matrix 
    Storage Manager et vous devez passer à l'étape 7 
    ci-dessous.

7.  Votre système ne semble pas fonctionner en mode RAID
    ou AHCI. Si vous pensez que votre système fonctionne
    en mode RAID ou AHCI et qu'aucun des contrôleurs
    ci-dessus n'est présent, contactez le fabricant de
    votre système ou le lieu d'achat pour obtenir
    de l'assistance.


************************************************************
* 5.  INSTALLATION DU LOGICIEL
************************************************************

5.1 Notes d'installation

1.  Si vous installez le système d'exploitation sur un 
    système configuré en mode RAID ou AHCI, vous devez 
    préinstaller le pilote Intel(R) Matrix Storage Manager
    en utilisant la méthode d'installation F6 décrite dans
    la section 5.3.

2.  L'Utilitaire d'installation du logiciel pour les jeux de 
    composants Intel(R) doit être installé sur le système 
    après l'installation d'un système d'exploitation 
    Microsoft* Windows* pris en charge.

3.  Pour installer Intel(R) Matrix Storage Manager,
    cliquez sur le fichier d'installation auto-extractible 
    et à installation automatique et suivez les invites qui 
    s'affichent.

4.  Par défaut, tous les fichiers installés (readme.txt, 
    aide, etc.) sont copiés à l'emplacement suivant : 
    
    <disque de démarrage>\Programmes\Intel\Intel(R) 
    Matrix Storage Manager

	
5.2 Installation Windows Automated Installer* à partir du
    disque dur ou du CD-ROM
    
REMARQUE : Cette méthode s'applique aux systèmes 
      	   configurés pour le mode RAID ou AHCI.

1.  Téléchargez le fichier d'installation Intel(R) Matrix 
    Storage Manager et double-cliquez sur ce fichier
    pour extraire automatiquement les fichiers et lancer le
    processus d'installation.

2.  La fenêtre de bienvenue s'affiche. Cliquez sur 
    Suivant pour continuer.

3.  La fenêtre d'avertissement de désinstallation s'affiche. 
    Cliquez sur Suivant pour continuer.

4.  La fenêtre de l'Accord de licence du logiciel s'affiche. 
    Si vous acceptez les termes de cet accord, cliquez sur
    Oui pour continuer.

5.  La fenêtre d'information sur le fichier Readme/Lisez-moi
    s'affiche. Cliquez sur Suivant pour continuer.

6.  La fenêtre de sélection de l'emplacement de destination
    s'affiche. Cliquez sur Suivant pour continuer.

7.  La fenêtre de sélection du dossier de programme s'affiche.  
    Cliquez sur Suivant pour continuer à installer
    le pilote.

8.  Si la fenêtre indiquant que l'assistant Windows Automated 
    Installer* est terminé s'affiche sans vous inviter à 
    redémarrer le système, cliquez sur Terminer et passez à 
    l'étape 8. Si une invite vous demande de redémarrer le 
    système, cliquez sur Oui, je veux redémarrer mon ordinateur 
    maintenant (sélection par défaut) et cliquez sur 
    Terminer. Après le redémarrage du système, passez à l'étape 8.

9.  Pour vérifier si le pilote est correctement chargé,
    reportez-vous à la section 6.


5.3 Préinstallation en utilisant la méthode F6 

REMARQUE : Les étapes 1 et 2 peuvent être ignorées si vous
      	   utilisez l'utilitaire de disquette F6 fourni par Intel.
           Ces méthodes sont applicables aux 
	   systèmes configurés pour le mode RAID ou AHCI.

1.  Extrayez tous les fichiers de pilote du package d'installation.
    Reportez-vous à la section 7.2 pour obtenir des
    instructions sur l'extraction des fichiers.

2.  Créez une disquette* contenant les fichiers suivants dans le
    répertoire racine :
    iaAhci.inf, iaAhci.cat,
    iaStor.inf, iaStor.cat,
    iaStor.sys et
    TxtSetup.oem. 

* REMARQUE : Pour Windows Vista vous pouvez utiliser une 
	     disquette, un CD/DVD ou un bus USB.

3.  Sous Windows XP ou les systèmes d'exploitation ultérieurs,

    - Au début de l'installation du système d'exploitation, appuyez
      sur F6 pour installer un pilote SCSI ou RAID tiers.

    - À l'invite, sélectionnez "S" pour spécifier un périphérique 
      supplémentaire.

    - Passez à l'étape 5.

4.  Sous Windows Vista :

    - Pendant l'installation du système d'exploitation, sélectionnez
      l'emplacement où vous souhaitez installer Vista, ensuite 
      cliquez sur Charger le pilote afin d'installer 
      un pilote SCSI ou RAID tiers.

    - Passez à l'étape 5.

5.  À l'invite, insérez la disquette, CD/DVD ou USB créé lors de 
    l'étape 2 et appuyez sur Entrée.

6.  Une sélection devrait maintenant s'afficher, vous
    permettant de sélectionner un des contrôleurs figurant
    dans la présentation (section 1) de ce document
    en fonction de la version matérielle et de la configuration.

7.  Mettez en surbrillance la sélection appropriée pour
    le matériel de votre système et appuyez sur Entrée.

8.  Appuyez de nouveau sur Entrée pour continuer. 
    Laissez la disquette dans le système jusqu'au prochain
    redémarrage car le logiciel devra être à nouveau copié
    de la disquette lorsque le programme d'installation
    copiera les fichiers.


************************************************************
* 6.  VÉRIFICATION DE L'INSTALLATION DU LOGICIEL
************************************************************

6.1 Vérification des installations Disquette fournie, F6 ou 
    sans assistance. 
    En fonction de la configuration de votre système,
    reportez-vous à la sous-rubrique appropriée ci-dessous :


6.1a Systèmes configurés pour le mode RAID :

1.  Dans le menu Démarrer :
    1a. Sous Windows* XP ou les systèmes d'exploitation 
        ultérieurs, sélectionnez Panneau de configuration.
2.  Ouvrez l'applet "Système" (vous devrez peut-être d'abord
    sélectionner "Basculer vers l'affichage classique").
3.  Sélectionnez l'onglet "Matériel" sous Windows* XP ou
    Windows* Server 2003.
4.  Sélectionnez le bouton "Gestionnaire de périphériques".
5.  Développez l'entrée "Contrôleurs de stockage" (sous Windows 
    Vista) ou "Contrôleurs SCSI et RAID" (sous Windows XP et 
    les systèmes d'exploitation ultérieurs).
6.  Cliquez avec le bouton droit sur "Intel(R) SATA 
    RAID Controller".
7.  Sélectionnez "Propriétés".
8.  Sélectionnez l'onglet "Pilote".
9.  Sélectionnez le bouton "Détails du pilote".
10. Si le fichier "iaStor.sys" est affiché, l'installation
    est réussie.


6.1b Systèmes configurés pour le mode AHCI :

1.  Dans le menu Démarrer :
    Sous Windows* XP ou les systèmes d'exploitation 
    ultérieurs, sélectionnez Panneau de configuration.
2.  Ouvrez l'applet "Système" (vous devrez peut-être d'abord
    sélectionner "Basculer vers l'affichage classique").
3.  Sélectionnez l'onglet "Matériel" sous Windows* XP ou
    Windows* Server 2003.
4.  Sélectionnez le bouton "Gestionnaire de périphériques".
5.  Développez l'entrée "Contrôleurs IDE ATA/ATAPI".
6.  Cliquez avec le bouton droit sur "Intel(R) SATA AHCI Controller".
7.  Sélectionnez "Propriétés".
8.  Sélectionnez l'onglet "Pilote".
9.  Sélectionnez le bouton "Détails du pilote".
10. Si le fichier "iaStor.sys" est affiché, l'installation
    est réussie.


6.2 Vérification des installations Windows Automated 
    Installer* ou "Package pour le Web" :

1.  Cliquez sur Démarrer.
2.  Recherchez le groupe de programmes "Intel(R) Matrix
    Storage Manager".
3.  Sélectionnez l'entrée "Intel(R) Matrix Storage Console".
4.  L'application "Intel(R) Matrix Storage Console" doit
    démarrer.
5.  Si cette application ne démarre pas, le pilote
    Intel(R) Matrix Storage Manager n'est pas installé
    correctement et le programme d'installation doit être 
    exécuté. 

************************************************************
* 7.  INSTRUCTIONS D'INSTALLATION AVANCÉES
************************************************************

7.1 Indicateurs d'installation disponibles :

    -?             Le programme d'installation affiche une boîte
		   de dialogue contenant tous les indicateurs 
		   d'installation pris en charge (affichés ici)
		   ainsi que leur utilisation.
    -A 		   Extrait tous les fichiers (n'installe pas le 
		   pilote) sous <chemin> si -P est également
                   fourni ; sinon, les fichiers sont extraits 
                   vers l'emplacement par défaut. 
    -B 		   Force un redémarrage du système après 
		   l'installation.
    -O <nom> 	   Permet de personnaliser le nom du dossier du 
                   programme pour Intel(R) Matrix Storage Console,
                   qui apparaît dans le menu Démarrer, "Tous les 
		   programmes".
    -P <chemin>    Fournit le chemin cible lorsqu'un indicateur 
		   -A est utilisé.
    -N 		   Installe tous les composants à l'exception du 
		   pilote.
    -NoGUI 	   Installe uniquement le pilote ; Intel(R) Matrix 
                   Storage Console, l'Observateur des événements et 
                   l'icône de la barre d'état système ne sont pas 
		   installés.
    -NoMon  	   Désactive l'Observateur des événements qui est 
                   constitué du service de surveillance de disque
                   et de l'application de l'icône de la barre d'état 
		   système.
    -S 		   Installation en mode silencieux (aucune 
		   invite utilisateur).
    -BUILD         Affiche les informations de version.		
    -G <numéro> 	   Force l'installation d'une langue particulière
		   (voir la section 3 pour la table de correspondance 
		   des <numéros> et des langues).
    -f2<chemin\nom> Créé un fichier journal sous le <chemin existant>
                   avec le <nom> ; à utiliser durant une installation
                   en mode silencieux. Les espaces ne sont pas 
                   autorisés entre -f2 et <chemin\nom> et le
		   chemin doit exister avant l'installation.

REMARQUE :  Les indicateurs et leurs paramètres ne sont pas 
	    sensibles à la casse.
            Les indicateurs peuvent être entrés dans n'importe
	    quel ordre, à l'exception de -S et -G qui doivent être
	    entrés en dernier. Si vous utilisez l'indicateur -A,
	    un chemin cible peut être spécifié via l'indicateur -P,
	    et les indicateurs -O, -G, -S et -N sont ignorés.
	    Lorsque vous utilisez les indicateurs -P, -O, -G et -f2,
	    aucun espace n'est autorisé entre l'indicateur et l'argument. 
	    Lorsque vous utilisez l'indicateur -f2, un nom de fichier 
	    journal et un chemin doivent être spécifiés, et le chemin 
	    doit exister avant l'installation.

7.2 Utilisez un des exemples de commande suivants pour
    extraire les fichiers de pilote des différents types 
    de package :

      c:\iata_cd.exe -a -a -pc:\<chemin>
      c:\iata_enu.exe -a -a -pc:\<chemin>
      c:\setup.exe -a -pc:\<chemin>

    L'exécution de ces commandes lance le processus 
    d'installation ; cliquez simplement dans les boîtes de 
    dialogue lorsque vous y êtes invité.
    Cette opération n'installe pas le pilote ; elle ne fait 
    qu'extraire les fichiers du pilote dans <chemin>. 
    Lorsque l'extraction est terminée, les fichiers du pilote 
    sont disponibles sous <chemin>\Driver.

7.3 Pour installer le pilote RAID sous Windows* XP, comme décrit
    dans le document Microsoft "Deployment Guide Automating
    Windows NT Setup", utilisez le fichier TXTSETUP.OEM inclus 
    dans ce package et insérez les lignes comme indiqué dans les
    étapes 7.3a et 7.3b dans le fichier UNATTEND.TXT. 
    Cette méthode est disponible pour Microsoft* Windows* XP,
    Windows 2000 et Windows Server 2003. Avant de commencer,
    les fichiers iaAhci.inf, iaAhci.cat, iaStor.inf, iaStor.cat,
    iaStor.sys et Txtsetup.oem doivent être extraits des fichiers
    d'installation. Pour extraire ces fichiers, utilisez la
    méthode décrite dans la section 7.2 ci-dessus.

7.3a Systèmes configurés pour le mode RAID :
    REMARQUE : Un exemple est montré ci-dessous. En fonction de
    votre version matérielle, veuillez mettre le texte à jour avec
    le nom exact du contrôleur RAID en utilisant la liste dans
    la présentation (section 1) de ce document.

    // Insérez les lignes suivantes dans le fichier UNATTEND.TXT
  
    [MassStorageDrivers]
    "Intel(R) 82801IR/IO SATA RAID Controller" = OEM
 
    [OEMBootFiles]
    iaStor.inf
    iaStor.sys
    iaStor.cat
    Txtsetup.oem


7.3b Systèmes configurés pour le mode AHCI :

    REMARQUE : Un exemple est montré ci-dessous. En fonction de
    votre version matérielle, veuillez mettre le texte à jour avec
    le nom exact du contrôleur AHCI en utilisant la liste dans
    la présentation (section 1) de ce document.

    // Insérez les lignes suivantes dans le fichier UNATTEND.TXT

    [MassStorageDrivers]
    "Intel(R) 82801IR/IO SATA AHCI Controller" = OEM
 
    [OEMBootFiles]
    iaAhci.inf
    iaStor.sys
    iaAhci.cat
    Txtsetup.oem


************************************************************
* 8.  IDENTIFICATION DU NUMÉRO DE VERSION DU LOGICIEL
************************************************************

8.1 Suivez les étapes ci-dessous pour identifier le numéro
    de version du logiciel à la suite d'une installation
    Disquette fournie, F6 ou sans assistance.


8.1a Systèmes configurés pour le mode RAID :

1.  Dans le menu Démarrer :
    1a. Sous Windows* XP ou les systèmes d'exploitation 
        ultérieurs, sélectionnez Panneau de configuration.
2.  Ouvrez l'applet "Système" (vous devrez peut-être d'abord
    sélectionner "Basculer vers l'affichage classique").
3.  Sélectionnez l'onglet "Matériel" sous Windows* XP ou
    Windows* Server 2003.
4.  Sélectionnez le bouton "Gestionnaire de périphériques".
5.  Développez l'entrée "Contrôleurs SCSI et RAID".
6.  Cliquez avec le bouton droit sur "Intel(R) RAID Controller".
7.  Sélectionnez "Propriétés".
8.  Sélectionnez l'onglet "Pilote".
9.  La version du logiciel est affichée après
    "Version du pilote".


8.1b Systèmes configurés pour le mode AHCI :

1.  Dans le menu Démarrer :
    1a. Sous Windows* XP ou les systèmes d'exploitation 
        ultérieurs, sélectionnez Panneau de configuration.
2.  Ouvrez l'applet "Système" (vous devrez peut-être d'abord
    sélectionner "Basculer vers l'affichage classique").
3.  Sélectionnez l'onglet "Matériel" sous Windows* XP ou
    Windows* Server 2003.
4.  Sélectionnez le bouton "Gestionnaire de périphériques".
5.  Développez l'entrée "Contrôleurs IDE ATA/ATAPI".
6.  Cliquez avec le bouton droit sur "Intel(R) SATA AHCI Controller".
7.  Sélectionnez "Propriétés".
8.  Sélectionnez l'onglet "Pilote".
9.  La version du logiciel est affichée après
    "Version du pilote".


8.2 Identifiez la version du logiciel pour les installations
    Windows Automated Installer* ou "Package pour le Web" :

1.  Cliquez sur Démarrer, puis sur Tous les programmes.
2.  Recherchez le groupe de programmes "Intel(R) Matrix
    Storage Manager".
3.  Sélectionnez l'élément "Intel(R) Matrix Storage Console".
4.  L'application "Intel(R) Matrix Storage Console" démarre,
    en affichant la version sur l'écran de démarrage. 
    La version peut également être affichée en sélectionnant
    "À propos de" dans le menu "Aide".


************************************************************
* 9.  DÉSINSTALLATION DU LOGICIEL
************************************************************

9a. DÉSINSTALLATION DES COMPOSANTS NON-PILOTE
Si vous supprimez ce logiciel du système, tous les disques
durs Serial ATA seront inaccessibles au système  
d'exploitation. Par conséquent, la désinstallation sera 
seulement pour les composants moins essentiels de ce logiciel
(l'interface utilisateur, liens dans le menu Démarrer, etc.). 
Pour désinstaller les composants essentiels, reportez-vous à 
la section 9b. 

Utilisez la procédure suivante pour désinstaller le logiciel :

1. Sélectionnez "Désinstaller" dans le dossier du menu 
   Démarrer suivant :

   * Tous les programmes -> Intel(R) Matrix Storage Manager

2. Le programme de désinstallation démarre. Cliquez sur les
   options appropriées pour déterminer la désinstallation.

9b. DÉSINSTALLATION DES COMPOSANTS PILOTE
Si vous supprimez ce logiciel du système, tous les disques
durs Serial ATA seront inaccessibles au système d'exploitation.
Par conséquent, il est conseillé de faire une copie de 
sauvegarde de vos données avant d'exécuter cette étape.
 
1) Si le système se trouve en mode RAID, supprimez les volumes
RAID, avec l'interface utilisateur d'Intel(R) Matrix
Storage Manager option ROM.
2) Redémarrez le système.
3) Entrez dans le BIOS du système (en appuyant sur "F2" ou
"Supprimer" pendant le démarrage du système).
4) Désactivez "Intel(R) RAID Technology" et "SATA AHCI mode".
5) Réinstallez le système d'exploitation.
 
REMARQUE : Si vous éprouvez des difficultés à modifier le BIOS
du système, contactez le fabricant de la carte mère pour 
obtenir de l'aide.
 
************************************************************
* 10.  OUVERTURE DE l'INTERFACE UTILISATEUR OPTION ROM
************************************************************

Suivez les étapes ci-dessous pour ouvrir l'interface 
utilisateur d'Intel(R) Matrix Storage Manager option ROM :

1. Démarrez le système.
2. Appuyez sur CTRL-I lorsque l'écran d'état
   "Intel(R) Matrix Storage Manager option 
   ROM vX.y.w.zzzz" s'affiche.

************************************************************
* 11.  GESTION DES VOLUMES RAID DANS L'OPTION ROM
************************************************************
Le composant Intel(R) Matrix Storage Manager option ROM 
permet de gérer les volumes RAID avant d'installer le système 
d'exploitation. L'interface utilisateur offre les options 
de gestion des volumes RAID suivantes :

1. Create RAID Volume (Créer un volume RAID)
   Utilisez cette option pour créer un ou deux 
   volumes RAID. 

2. Delete RAID Volume (Supprimer un volume RAID)
   Utilisez cette option pour supprimer un volume RAID.

3. Reset Disks to Non-RAID (Réinitialiser les disques durs sur Non RAID)
   Utilisez cette option pour réinitialiser une
   configuration RAID avec une configuration non RAID.

4. Recovery Volume Options (Options du volume de reprise)
   Si le système comporte un volume de reprise, utilisez 
   cette option pour :
        a. Disable Continuous Update (Désactiver la mise à jour continue)
        b. Enable Only Recovery Disk (Démarrer sur un disque de reprise)
        c. Enable Only Master Disk (Démarrer sur un disque maître)

************************************************************
* 12.  OPTIONS DE RÉINITIALISATION DU VOLUME RAID DANS L'OPTION ROM
************************************************************
L'interface utilisateur d'Intel(R) Matrix Storage option ROM 
propose deux méthodes pour réinitialiser les volumes RAID :
1. Delete RAID Volume (Supprimer un volume RAID)
2. Reset Disks to Non-RAID (Réinitialiser les disques durs sur Non RAID)
   Les différences entre les options sont notées ci-dessous. 
   Les utilisateurs sont conseillés de choisir l'option en
   fonction de la situation.

12.1 Suppression d'un volume RAID

     Quand un volume RAID est supprimé, les métadonnées sur le
     disque sont effacées et le secteur zéro est supprimé, ce
     qui signifie que les données de la table de partition et du
     système de fichiers sont effacées. L'installateur de Windows 
     ne trouvera aucune donnée inadmissible pendant 
     l'installation du système d'exploitation. C'est la méthode 
     recommandée pour modifier le volume RAID et installer le
     système d'exploitation.

12.2 Réinitialisation du disque sur Non RAID

     Cette option est employée pour réinitialiser les métadonnées
     sur le disque qui participe à plus d'un volume RAID dans une 
     seule opération. Il devrait être employé si l'option
     "Effacer le volume RAID'" échoue pour une raison ou une autre
     et pour réinitialiser un disque qui a été marqué Disponible et 
     en différé. Quand un disque en volume RAID est réinitialisé
     comme non-RAID, les métadonnées RAID sont effacées. 
     Cependant, les données de la table de partition et du système 
     de fichiers existent toujours, ce qui peut être inadmissible. 
     L'installateur de Windows pourrait mal interpréter l'information
     disponible sur le "disque de réinstallation" au moment de 
     l'installation. Ceci peut avoir comme conséquence un comportement 
     inattendu dans l'installation du système d'exploitation.

************************************************************
* 13.  VÉRIFICATION DE LA VERSION DU LOGICIEL OPTION ROM
************************************************************

1. Suivez les étapes ci-dessous pour identifier le numéro de
   version de l'interface utilisateur RAID option ROM :

   - Ouvrez l'interface utilisateur RAID option ROM en
     suivant les étapes décrites dans la section 10.
   - La version du logiciel sera affichée dans la bannière 
     de l'interface utilisateur :
     "Intel(R) Matrix Storage Manager option ROM vX.y.w.zzzz".

     "X.y.w.zzzz" - correspond au numéro de version de 
     l'interface utilisateur d'Intel(R) Matrix Storage option ROM
     installée sur votre système :
     "X.y.w" - Numéro de lancement du produit
     "X" - Numéro majeur
     "y" - Numéro mineur
     "w" - Numéro de correction à chaud
     "zzzz" - Numéro de compilation

************************************************************
* AVIS DE NON-RESPONSABILITÉ
************************************************************

Les informations de ce document sont fournies en relation
avec les produits Intel. Sauf disposition expressément
stipulée dans le CONTRAT DE LICENCE DU LOGICIEL INTEL
contenu dans ce document, aucune licence n'est accordée, 
expressément ou implicitement, par estoppel ou autre,
sur un droit de propriété intellectuelle quel qu'il soit.
Sauf disposition expressément stipulée par Intel dans les 
Modalités et conditions de vente de ces produits, Intel
décline toute responsabilité quelle qu'elle soit et exclut
toute garantie expresse ou implicite relative à la vente
et/ou à l'utilisation de produits Intel, y compris toute
responsabilité ou garantie relative à l'adaptation à un
usage particulier, à la qualité marchande ou au respect
d'un brevet, d'un droit d'auteur ou de tout autre droit 
de propriété intellectuelle. Les produits Intel ne sont pas 
conçus pour être utilisés dans des applications médicales, 
de secours ou de réanimation.

************************************************************
* Intel Corporation exclut toutes garanties et
* responsabilités relatives à l'utilisation de ce document,
* au logiciel et aux informations contenues dans ce
* document, et décline toute responsabilité dans le cas
* où des erreurs apparaîtraient dans ce document ou dans le
* logiciel, et Intel ne s'engage aucunement à mettre à jour 
* les informations ou le logiciel contenu dans ce document.
* Intel se réserve le droit de modifier le présent document
* ou le logiciel à tout moment et sans préavis.
************************************************************

* D'autres noms et marques peuvent appartenir à leurs
  propriétaires respectifs.

Copyright (c) Intel Corporation, 2001-2008
************************************************************
* CONTRAT DE LICENCE DU LOGICIEL INTEL
************************************************************
ACCORD DE LICENCE DU LOGICIEL INTEL (distribution OEM /IHV/ ISV et mono-utilisateur)

IMPORTANT - � LIRE AVANT DE COPIER, D'INSTALLER OU D'UTILISER LE LOGICIEL
Lisez attentivement les termes et conditions du pr�sent contrat de licence avant d'utiliser ou de charger le pr�sent logiciel et tout le mat�riel associ� (appel�s collectivement le "logiciel"). L'utilisation ou le chargement du logiciel constitue une acceptation des termes du pr�sent contrat. En cas de refus de ces termes, n'installez pas le logiciel et ne l'utilisez pas.

Autre remarque importante :
* Si vous �tes fabricant de mat�riel d'origine (OEM), fournisseur de mat�riel ind�pendant (IHV) ou fournisseur de logiciel ind�pendant (ISV), l'ensemble du pr�sent CONTRAT DE LICENCE s'applique.
* Si vous �tes utilisateur final, seul le document A, ACCORD DE LICENCE DU LOGICIEL INTEL, s'applique.

Pour OEM, IHV et ISV:

LICENCE. La licence de ce logiciel est accord�e pour une utilisation exclusive de ce dernier avec des composants Intel. L'utilisation de ce logiciel avec des composants n'appartenant pas � Intel n'est pas couverte par la pr�sente licence. Sous r�serve des modalit�s de cet accord, Intel vous conc�de une licence non exclusive, incessible, valide dans le monde entier et enti�rement pay�e vous autorisant �:
	a) utiliser, modifier et copier le logiciel en interne, � vos propres fins de d�veloppement et de maintenance ;
	b) modifier, copier et distribuer le logiciel, y compris les travaux qui en sont d�riv�s, � vos utilisateurs finals, mais uniquement en vertu d'un accord de licence dont les modalit�s sont au moins aussi restrictives que celles de l'accord de licence de l'utilisateur final Intel, ci-joint � titre de document A ; et
	c) modifier, copier et distribuer la documentation de l'utilisateur final qui peut accompagner le logiciel, mais uniquement avec le logiciel.

Si vous n'�tes pas le fabricant ou fournisseur final d'un syst�me informatique ou d'un programme int�grant le logiciel, vous pouvez transf�rer une copie du logiciel, y compris les travaux qui en sont d�riv�s (et la documentation connexe de l'utilisateur final), � une tierce partie qui pourra l'utiliser conform�ment aux modalit�s du pr�sent accord, � condition qu'elle accepte pleinement d'�tre li�e par celles-ci. Sauf dans le cas pr�sent� pr�c�demment, vous n'�tes pas habilit� � c�der, conc�der en vertu d'une sous-licence, louer, transf�rer ni divulguer le logiciel � un tiers quelconque. Vous ne pouvez pas d�compiler, ou d�sassembler le logiciel ou le soumettre � un processus d'ing�nierie � rebours.

Sauf mention expresse dans le pr�sent accord, aucun droit ni licence ne vous est accord� de mani�re directe ou tacite, par incitation, par forclusion ou autrement. Intel se r�serve le droit d'inspecter ou de faire inspecter par un v�rificateur ind�pendant tous vos dossiers pertinents afin de v�rifier si vous respectez les modalit�s et conditions du pr�sent accord.

CONFIDENTIALIT�. Si vous d�sirez qu'un conseiller ou sous-traitant tiers (ci-apr�s d�nomm� "entrepreneur") ex�cute pour vous des travaux n�cessitant l'utilisation du logiciel ou l'acc�s � ce dernier, vous devez obtenir de l'entrepreneur une convention �crite de confidentialit� dont les modalit�s et les obligations relatives � l'acc�s au logiciel et � son utilisation sont au moins aussi restrictives que celles du pr�sent accord, et qui excluent tout droit de distribution et d'utilisation � d'autres fins.
Par ailleurs, vous n'�tes pas habilit� � divulguer les modalit�s ou l'existence de cet accord ni � utiliser le nom Intel dans des publications, des publicit�s ou d'autres annonces sans obtenir l'autorisation �crite pr�alable d'Intel. Vous ne pouvez pas utiliser les marques commerciales d'Intel.

PROPRI�T� DU LOGICIEL ET DROITS D'AUTEUR. Les droits sur toutes les copies du logiciel demeurent la propri�t� d'Intel ou de ses fournisseurs. Le logiciel est soumis � droits d'auteur et prot�g� par les lois des �tats-Unis et d'autres pays ainsi que par les dispositions de trait�s internationaux. Vous n'�tes pas autoris� � �ter les mentions de droit d'auteur du logiciel. Intel peut modifier, � tout moment et sans pr�avis, le logiciel ou les �l�ments qui y sont mentionn�s, mais n'est pas tenu � des services d'assistance relatifs au logiciel ou � la mise � jour de ce dernier. Sauf stipulation contraire expresse, Intel n'accorde aucun droit expr�s ou tacite en vertu des brevets, droits d'auteur, marques commerciales ou autres droits de propri�t� intellectuelle d'Intel. Vous ne pouvez transf�rer le logiciel que si le destinataire convient d'�tre enti�rement li� par les dispositions du pr�sent accord et si vous ne conservez aucune copie du logiciel.

GARANTIE LIMIT�E DES SUPPORTS. Si le logiciel a �t� livr� par Intel sur des supports physiques, Intel garantit que ces derniers sont exempts de vices mat�riels pendant une p�riode de quatre-vingt-dix (90) jours � compter de la date de livraison par Intel. En cas de d�faut de support, vous �tes invit� � renvoyer ce dernier � Intel pour un remplacement ou une autre livraison du logiciel, � la discr�tion d'Intel.

EXCLUSION DES AUTRES GARANTIES. � L'EXCEPTION DES GARANTIES QUI PR�C�DENT, LE LOGICIEL EST FOURNI "EN L'�TAT", SANS GARANTIE EXPRESSE OU TACITE DE QUELQUE NATURE QUE CE SOIT, Y COMPRIS LES GARANTIES CONCERNANT LA VALEUR MARCHANDE, L'ABSENCE DE CONTREFA�ON OU L'AD�QUATION � UN USAGE PARTICULIER. Intel ne garantit pas l'exactitude ni l'exhaustivit� des informations, textes, graphiques, liens et autres �l�ments int�gr�s � ce logiciel et n'assume aucune responsabilit� � cet �gard.

LIMITATION DE LA RESPONSABILIT�. INTEL OU SES FOURNISSEURS NE SONT EN AUCUN CAS RESPONSABLES DE QUELQUE DOMMAGE QUE CE SOIT (Y COMPRIS, MAIS SANS QUE CETTE �NUM�RATION SOIT LIMITATIVE, LES PERTES DE B�N�FICES, LES INTERRUPTIONS D'ACTIVIT�S OU LES PERTES D'INFORMATIONS) D�RIVANT DE L'UTILISATION DE CE PRODUIT OU DE L'INCAPACIT� DE L'UTILISER, M�ME SI INTEL A �T� NOTIFI� DE LA POSSIBILIT� D'UN TEL DOMMAGE. CERTAINS RESSORTS INTERDISENT L'EXCLUSION OU LA LIMITATION DE LA RESPONSABILIT� POUR LES GARANTIES TACITES OU LES DOMMAGES INDIRECTS OU ACCESSOIRES. IL SE PEUT PAR CONS�QUENT QUE LES LIMITATIONS SUSMENTIONN�ES NE S'APPLIQUENT PAS DANS VOTRE CAS. LES AUTRES DROITS DONT VOUS JOUISSEZ PEUVENT VARIER D'UN RESSORT � L'AUTRE.

R�SILIATION DU PR�SENT ACCORD. Intel peut d�noncer le pr�sent accord � tout moment en cas de violation des dispositions qu'il contient. Le cas �ch�ant, vous �tes tenu de proc�der � la destruction imm�diate du logiciel ou d'en renvoyer tous les exemplaires � Intel.
 
DROIT APPLICABLE. Les litiges n�s du pr�sent accord sont r�gis par les lois de l'�tat de Californie, sans tenir compte des principes de conflit de lois et de la Convention des Nations Unies sur les accords de vente de marchandises. Vous ne pouvez pas exporter le logiciel en contravention des lois et r�glements en vigueur sur l'exportation. Intel n'est li� par aucun autre accord, � moins que ce dernier soit sous forme �crite et sign� par un repr�sentant agr�� d'Intel.

LIMITATION DES DROITS DU GOUVERNEMENT. Le logiciel est fourni avec des "DROITS LIMIT�S". L'utilisation, la reproduction ou la publication par le gouvernement est soumise aux restrictions d�finies dans les articles FAR52.227-14 et DFAR252.227-7013 et suivants, ou leurs successeurs. L'utilisation du logiciel par le gouvernement constitue une reconnaissance des droits de propri�t� y aff�rents d'Intel. L'entrepreneur ou le fabricant est Intel Corporation, 2200 Mission College Blvd., Santa Clara, CA 95052, USA.


DOCUMENT A

ACCORD DE LICENCE DU LOGICIEL INTEL (version finale, mono-utilisateur)

IMPORTANT - � LIRE AVANT DE COPIER, D'INSTALLER OU D'UTILISER LE LOGICIEL
Lisez attentivement les termes et conditions du pr�sent accord de licence avant d'utiliser ou de charger le pr�sent logiciel et tout le mat�riel associ� (appel�s collectivement le "logiciel"). L'utilisation ou le chargement du logiciel constitue une acceptation des termes du pr�sent accord. En cas de refus de ces termes, n'installez pas le logiciel et ne l'utilisez pas.

LICENCE. Vous pouvez copier le logiciel sur un seul ordinateur pour une utilisation personnelle et non commerciale et en effectuer une copie de sauvegarde, sous r�serve des conditions suivantes :

1. La licence de ce logiciel est accord�e pour une utilisation exclusive de ce dernier avec des composants Intel. L'utilisation de ce logiciel avec des composants n'appartenant pas � Intel n'est pas couverte par la pr�sente licence.
2. Vous ne pouvez pas copier, modifier, louer, vendre, distribuer ou transf�rer aucune partie du logiciel, sauf tel qu'il est stipul� aux pr�sentes, et vous vous engagez � emp�cher toute reproduction non autoris�e du logiciel.
3. Vous ne pouvez pas d�compiler ni d�sassembler le logiciel. 
4. Vous ne pouvez pas conc�der le logiciel en vertu d'une sous-licence ni en autoriser l'utilisation simultan�e par plusieurs utilisateurs.
5. Le logiciel peut contenir des programmes et autres �l�ments qui sont la propri�t� de tiers fournisseurs, dont certains peuvent �tre identifi�s dans un fichier "license.txt" ou d'autres textes ou fichiers inclus et conc�d�s sous licence en vertu de ceux-ci.

PROPRI�T� DU LOGICIEL ET DROITS D'AUTEUR. Les droits sur toutes les copies du logiciel demeurent la propri�t� d'Intel ou de ses fournisseurs. Le logiciel est soumis � droits d'auteur et prot�g� par les lois des �tats-Unis et d'autres pays ainsi que par les dispositions de trait�s internationaux. Vous n'�tes pas autoris� � �ter les mentions de droit d'auteur du logiciel. Intel peut modifier, � tout moment et sans pr�avis, le logiciel ou les �l�ments qui y sont mentionn�s, mais n'est pas tenu � des services d'assistance relatifs au logiciel ou � la mise � jour de ce dernier. Sauf stipulation contraire expresse, Intel n'accorde aucun droit expr�s ou tacite en vertu des brevets, droits d'auteur, marques commerciales ou autres droits de propri�t� intellectuelle d'Intel. Vous ne pouvez transf�rer le logiciel que si le destinataire convient d'�tre enti�rement li� par les dispositions du pr�sent accord et si vous ne conservez aucune copie du logiciel.

GARANTIE LIMIT�E DES SUPPORTS. Si le logiciel a �t� livr� par Intel sur des supports physiques, Intel garantit que ces supports sont exempts de vices mat�riels pendant une p�riode de quatre-vingt-dix (90) jours � compter de la date de livraison par Intel. En cas de d�faut de support, vous �tes invit� � renvoyer ce dernier � Intel pour un remplacement ou une autre livraison du logiciel, � la discr�tion d'Intel.

EXCLUSION DES AUTRES GARANTIES. � L'EXCEPTION DES GARANTIES QUI PR�C�DENT, LE LOGICIEL EST FOURNI "EN L'�TAT", SANS GARANTIE EXPRESSE OU TACITE DE QUELQUE NATURE QUE CE SOIT, Y COMPRIS LES GARANTIES CONCERNANT LA VALEUR MARCHANDE, L'ABSENCE DE CONTREFA�ON OU L'AD�QUATION � UN USAGE PARTICULIER. Intel ne garantit pas ni l'exactitude ni l'exhaustivit� des informations, textes, graphiques, liaisons et autres �l�ments int�gr�s � ce logiciel et n'assume aucune responsabilit� � cet �gard.

LIMITATION DE LA RESPONSABILIT�. INTEL OU SES FOURNISSEURS NE SONT EN AUCUN CAS RESPONSABLES DE QUELQUE DOMMAGE QUE CE SOIT (Y COMPRIS, MAIS SANS QUE CETTE �NUM�RATION SOIT LIMITATIVE, LES PERTES DE B�N�FICE, LES INTERRUPTIONS D'ACTIVIT�S OU LES PERTES D'INFORMATIONS) D�RIVANT DE L'UTILISATION DE CE PRODUIT OU DE L'INCAPACIT� DE L'UTILISER, M�ME SI INTEL A �T� NOTIFI� DE LA POSSIBILIT� D'UN TEL DOMMAGE. CERTAINS RESSORTS INTERDISENT L'EXCLUSION OU LA LIMITATION DE LA RESPONSABILIT� POUR LES GARANTIES TACITES OU DES DOMMAGES INDIRECTS OU ACCESSOIRES. IL SE PEUT PAR CONS�QUENT QUE LES LIMITATIONS SUSMENTIONN�ES NE S'APPLIQUENT PAS DANS VOTRE CAS. LES AUTRES DROITS L�GAUX DONT VOUS JOUISSEZ PEUVENT VARIER D'UN RESSORT � L'AUTRE.

R�SILIATION DU PR�SENT ACCORD. Intel peut d�noncer le pr�sent accord � tout moment en cas de violation des dispositions qu'il contient. Le cas �ch�ant, vous �tes tenu de proc�der � la destruction imm�diate du logiciel ou d'en renvoyer tous les exemplaires � Intel.
 
DROIT APPLICABLE. Les litiges n�s du pr�sent accord sont r�gis par les lois de l'�tat de Californie, sans tenir compte des principes de conflit de lois et de la Convention des Nations Unies sur les accords de vente de marchandises. Vous ne pouvez pas exporter le logiciel en contravention des lois et r�glements en vigueur sur l'exportation. Intel n'est li� par aucun autre accord, � moins que ce dernier soit sous forme �crite et sign� par un repr�sentant agr�� d'Intel.

LIMITATION DES DROITS DU GOUVERNEMENT. Le logiciel est fourni avec des "DROITS LIMIT�S". L'utilisation, la reproduction ou la publication par le gouvernement est soumise aux restrictions d�finies dans les articles FAR52.227-14 et DFAR252.227-7013 et suivants, ou leurs successeurs. L'utilisation du logiciel par le gouvernement constitue une reconnaissance des droits de propri�t� y aff�rents d'Intel. L'entrepreneur ou fabricant est Intel Corporation, 2200 Mission College Blvd., Santa Clara, CA 95052, USA.
SLAOEMISV1/RBK/01-21-22

LANGUE ; TRADUCTIONS.  Au cas o� la version anglaise du pr�sent Accord est accompagn�e d'une version traduite dans une autre langue, la version traduite est fournie � titre d'information uniquement et la version anglaise constituera la version de r�f�rence.



INTEL SOFTWARE LICENSE AGREEMENT (OEM / IHV / ISV Distribution & Single User)

IMPORTANT - READ BEFORE COPYING, INSTALLING OR USING. 
Do not use or load this software and any associated materials (collectively, the "Software") until you have carefully read the following terms and conditions. By loading or using the Software, you agree to the terms of this Agreement. If you do not wish to so agree, do not install or use the Software.

Please Also Note:
* If you are an Original Equipment Manufacturer (OEM), Independent Hardware Vendor (IHV), or Independent Software Vendor (ISV), this complete LICENSE AGREEMENT applies;
* If you are an End-User, then only Exhibit A, the INTEL SOFTWARE LICENSE AGREEMENT, applies.

For OEMs, IHVs, and ISVs:

LICENSE. This Software is licensed for use only in conjunction with Intel component products.  Use of the Software in conjunction with non-Intel component products is not licensed hereunder. Subject to the terms of this Agreement, Intel grants to you a nonexclusive, nontransferable, worldwide, fully paid-up license under Intel's copyrights to:
	a) use, modify and copy Software internally for your own development and maintenance purposes; and
	b) modify, copy and distribute Software, including derivative works of the Software, to your end-users, but only under a license agreement with terms at least as restrictive as those contained in Intel's Final, Single User License Agreement, attached as Exhibit A; and
	c) modify, copy and distribute the end-user documentation which may accompany the Software, but only in association with the Software.

If you are not the final manufacturer or vendor of a computer system or software program incorporating the Software, then you may transfer a copy of the Software, including derivative works of the Software (and related end-user documentation) to your recipient for use in accordance with the terms of this Agreement, provided such recipient agrees to be fully bound by the terms hereof.  You shall not otherwise assign, sublicense, lease, or in any other way transfer or disclose Software to any third party. You shall not reverse- compile, disassemble or otherwise reverse-engineer the Software.

Except as expressly stated in this Agreement, no license or right is granted to you directly or by implication, inducement, estoppel or otherwise.  Intel shall have the right to inspect or have an independent auditor inspect your relevant records to verify your compliance with the terms and conditions of this Agreement.

CONFIDENTIALITY. If you wish to have a third party consultant or subcontractor ("Contractor") perform work on your behalf which involves access to or use of Software, you shall obtain a written confidentiality agreement from the Contractor which contains terms and obligations with respect to access to or use of Software no less restrictive than those set forth in this Agreement and excluding any distribution rights, and use for any other purpose.
Otherwise, you shall not disclose the terms or existence of this Agreement or use Intel's name in any publications, advertisements, or other announcements without Intel's prior written consent.  You do not have any rights to use any Intel trademarks or logos.

OWNERSHIP OF SOFTWARE AND COPYRIGHTS. Title to all copies of the Software remains with Intel or its suppliers. The Software is copyrighted and protected by the laws of the United States and other countries, and international treaty provisions. You may not remove any copyright notices from the Software. Intel may make changes to the Software, or to items referenced therein, at any time and without notice, but is not obligated to support or update the Software. Except as otherwise expressly provided, Intel grants no express or implied right under Intel patents, copyrights, trademarks, or other intellectual property rights. You may transfer the Software only if the recipient agrees to be fully bound by these terms and if you retain no copies of the Software.

LIMITED MEDIA WARRANTY. If the Software has been delivered by Intel on physical media, Intel warrants the media to be free from material physical defects for a period of ninety (90) days after delivery by Intel. If such a defect is found, return the media to Intel for replacement or alternate delivery of the Software as Intel may select.

EXCLUSION OF OTHER WARRANTIES. EXCEPT AS PROVIDED ABOVE, THE SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY EXPRESS OR IMPLIED WARRANTY OF ANY KIND, INCLUDING WARRANTIES OF MERCHANTABILITY, NONINFRINGEMENT, OR FITNESS FOR A PARTICULAR PURPOSE.  Intel does not warrant or assume responsibility for the accuracy or completeness of any information, text, graphics, links or other items contained within the Software.

LIMITATION OF LIABILITY. IN NO EVENT SHALL INTEL OR ITS SUPPLIERS BE LIABLE FOR ANY DAMAGES WHATSOEVER (INCLUDING, WITHOUT LIMITATION, LOST PROFITS, BUSINESS INTERRUPTION OR LOST INFORMATION) ARISING OUT OF THE USE OF OR INABILITY TO USE THE SOFTWARE, EVEN IF INTEL HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. SOME JURISDICTIONS PROHIBIT EXCLUSION OR LIMITATION OF LIABILITY FOR IMPLIED WARRANTIES OR CONSEQUENTIAL OR INCIDENTAL DAMAGES, SO THE ABOVE LIMITATION MAY NOT APPLY TO YOU. YOU MAY ALSO HAVE OTHER LEGAL RIGHTS THAT VARY FROM JURISDICTION TO JURISDICTION. 

TERMINATION OF THIS AGREEMENT. Intel may terminate this Agreement at any time if you violate its terms. Upon termination, you will immediately destroy the Software or return all copies of the Software to Intel.
 
APPLICABLE LAWS. Claims arising under this Agreement shall be governed by the laws of California, excluding its principles of conflict of laws and the United Nations Convention on Contracts for the Sale of Goods. You may not export the Software in violation of applicable export laws and regulations. Intel is not obligated under any other agreements unless they are in writing and signed by an authorized representative of Intel.

GOVERNMENT RESTRICTED RIGHTS. The Software is provided with "RESTRICTED RIGHTS." Use, duplication, or disclosure by the Government is subject to restrictions as set forth in FAR52.227-14 and DFAR252.227-7013 et seq. or their successors. Use of the Software by the Government constitutes acknowledgment of Intel's proprietary rights therein. Contractor or Manufacturer is Intel Corporation, 2200 Mission College Blvd., Santa Clara, CA 95052.


EXHIBIT "A" 
INTEL SOFTWARE LICENSE AGREEMENT (Final, Single User)

IMPORTANT - READ BEFORE COPYING, INSTALLING OR USING. 
Do not use or load this software and any associated materials (collectively, the "Software") until you have carefully read the following terms and conditions. By loading or using the Software, you agree to the terms of this Agreement. If you do not wish to so agree, do not install or use the Software.

LICENSE. You may copy the Software onto a single computer for your personal, noncommercial use, and you may make one back-up copy of the Software, subject to these conditions: 
1. This Software is licensed for use only in conjunction with Intel component products.  Use of the Software in conjunction with non-Intel component products is not licensed hereunder. 
2. You may not copy, modify, rent, sell, distribute or transfer any part of the Software except as provided in this Agreement, and you agree to prevent unauthorized copying of the Software.
3. You may not reverse engineer, decompile, or disassemble the Software. 
4. You may not sublicense or permit simultaneous use of the Software by more than one user.
5. The Software may contain the software or other property of third party suppliers, some of which may be identified in, and licensed in accordance with, any enclosed "license.txt" file or other text or file. 

OWNERSHIP OF SOFTWARE AND COPYRIGHTS. Title to all copies of the Software remains with Intel or its suppliers. The Software is copyrighted and protected by the laws of the United States and other countries, and international treaty provisions. You may not remove any copyright notices from the Software. Intel may make changes to the Software, or to items referenced therein, at any time without notice, but is not obligated to support or update the Software. Except as otherwise expressly provided, Intel grants no express or implied right under Intel patents, copyrights, trademarks, or other intellectual property rights. You may transfer the Software only if the recipient agrees to be fully bound by these terms and if you retain no copies of the Software.

LIMITED MEDIA WARRANTY. If the Software has been delivered by Intel on physical media, Intel warrants the media to be free from material physical defects for a period of ninety (90) days after delivery by Intel. If such a defect is found, return the media to Intel for replacement or alternate delivery of the Software as Intel may select.

EXCLUSION OF OTHER WARRANTIES EXCEPT AS PROVIDED ABOVE, THE SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY EXPRESS OR IMPLIED WARRANTY OF ANY KIND INCLUDING WARRANTIES OF MERCHANTABILITY, NONINFRINGEMENT, OR FITNESS FOR A PARTICULAR PURPOSE.  Intel does not warrant or assume responsibility for the accuracy or completeness of any information, text, graphics, links or other items contained within the Software.

LIMITATION OF LIABILITY.  IN NO EVENT SHALL INTEL OR ITS SUPPLIERS BE LIABLE FOR ANY DAMAGES WHATSOEVER (INCLUDING, WITHOUT LIMITATION, LOST PROFITS, BUSINESS INTERRUPTION, OR LOST INFORMATION) ARISING OUT OF THE USE OF OR INABILITY TO USE THE SOFTWARE, EVEN IF INTEL HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. SOME JURISDICTIONS PROHIBIT EXCLUSION OR LIMITATION OF LIABILITY FOR IMPLIED WARRANTIES OR CONSEQUENTIAL OR INCIDENTAL DAMAGES, SO THE ABOVE LIMITATION MAY NOT APPLY TO YOU. YOU MAY ALSO HAVE OTHER LEGAL RIGHTS THAT VARY FROM JURISDICTION TO JURISDICTION. 

TERMINATION OF THIS AGREEMENT. Intel may terminate this Agreement at any time if you violate its terms. Upon termination, you will immediately destroy the Software or return all copies of the Software to Intel.
 
APPLICABLE LAWS. Claims arising under this Agreement shall be governed by the laws of California, excluding its principles of conflict of laws and the United Nations Convention on Contracts for the Sale of Goods. You may not export the Software in violation of applicable export laws and regulations. Intel is not obligated under any other agreements unless they are in writing and signed by an authorized representative of Intel.

GOVERNMENT RESTRICTED RIGHTS. The Software is provided with "RESTRICTED RIGHTS." Use, duplication, or disclosure by the Government is subject to restrictions as set forth in FAR52.227-14 and DFAR252.227-7013 et seq. or their successors. Use of the Software by the Government constitutes acknowledgment of Intel's proprietary rights therein. Contractor or Manufacturer is Intel Corporation, 2200 Mission College Blvd., Santa Clara, CA 95052.
 
SLAOEMISV1/RBK/01-21-00


