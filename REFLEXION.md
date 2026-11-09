# Réflexion : SEO technique

1. **Non.** `robots.txt` contrôle l'exploration, pas la déduplication. Si Google
   trouve un lien externe vers une URL bloquée, il peut tout de même l'indexer
   sans en explorer le contenu.

2. **La balise canonique indique l'URL de référence** parmi plusieurs pages au
   contenu identique ou similaire. `robots.txt` ne donne pas cette indication,
   tandis que `noindex` demanderait de retirer une page des résultats au lieu de
   regrouper les variantes autour de l'URL principale.

3. Ajouter `Disallow: /admin` sous le groupe `User-agent: *` dans
   `robots.txt`.
