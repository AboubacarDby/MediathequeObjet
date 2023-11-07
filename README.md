# MediathequeObjet

package mediatheque;

public class MediathequeObjet {

    public static void main(String[] args) {
	Abonnement passSimple = new Abonnement("simple", 4, false);
	Abonnement passMulti = new Abonnement("multimédia", 8, true);
	Lecteur lecteur = new Lecteur("Jean", "Dupont", 1, passSimple);
	System.out.println("Voici la description du lecteur : " + lecteur.getPrenom() + " " + lecteur.getNom() + " "
		+ lecteur.getNumAdhe() + " " + passSimple.getNomAbo());
	Bibliothecaire bibliothecaire = new Bibliothecaire("Michelle", "Lelong");
	Emplct emplctJeux = new Emplct(1, 1, "Jeux");
	Emplct emplctLivres = new Emplct(1, 2, "Livres");
	Jeux jeuCatane = new Jeux("Catane", "Paolo Paola", 1, emplctJeux, CategoriesJeux.STR);
	Jeux jeuUno = new Jeux("Uno", "Frantz Licht", 2, emplctJeux, CategoriesJeux.FAM);
	Livres livreCarrie = new Livres("Carrie", "Stephen King", 1, emplctLivres, CategoriesLivres.POL,
		"978-2-11-224-4");
	Livres livre = new Livres("L'amour est dans le Pré", "Penelope Douglas", 2, emplctLivres, CategoriesLivres.ROM,
		"978-2-11-226-4");

    }

}
