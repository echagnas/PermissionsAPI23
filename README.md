# PermissionsAPI23

Example d'utilisation des permissions introduit avec Android 6.0.

Dorénavant, les permissions ne sont plus demandées à l'installation, mais pendant l'exécution du programme.
Nous devons donc tester, avant d'appeler la méthode qui a besoin de cette permission, si l'utilisateur à 
accepter la permission ou non. S'il n'a pas la permission, on lui affiche le message système qui lui demande 
d'accepter ou de refuser. S'il a déjà refusée une première fois, ce message comportera une coche en plus
"ne plus me demander". S'il refuse encore, on lui affiche alors un message spécifique à l'application
qui lui explique plus précisemment pourquoi on lui demande cette permission. Cette explication est très 
importante, car elle explique la demande de permission dans un contexte bien précis.
Si l'utilisateur refuse, il faut alors adapter l'application en fonction. Si c'est une permission pour pouvoir 
effectuer des appels téléphoniques par exemple, alors l'application ne pourra pas en faire...

L'explication que j'ai mis dans mon exemple est basé sur cce qu'à fait Google dans l'application Google Maps.
La popup comporte 2 boutons, l'un revient et redemande la permission, l'autre ferme la popup tout simplement.
