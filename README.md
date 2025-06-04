# *🧪 Analyse de la variance (ANOVA)*
# *🎯 Objectif*
  * Rémi, passionné de philatélie, souhaite savoir si l’épaisseur moyenne des timbres varie selon leur pays d’origine (Allemagne, Autriche, Belgique, France).

# *📊 Étapes de l’analyse*
# *1. Importation des données*
    * Fichier utilisé : timbres.csv
    * Colonnes : pays, epaisseur
# *2. Statistiques descriptives*
    * Moyenne, écart-type, min, max, etc. par pays.
# *3. Hypothèses*
    * H₀ : Les moyennes d’épaisseur sont égales entre les pays.
    * H₁ : Au moins une moyenne diffère.
# *4. Conditions d’application*
    ✅ Normalité (Shapiro-Wilk) : p-valeurs > 0,05 → normalité acceptée.
    ✅ Homogénéité des variances (Bartlett) : p = 0,3838 > 0,05 → variances égales.
# *5. Test ANOVA*
    * Statistique F : 194,62
    * p-valeur : < 0,05
    ✅ Résultat : H₀ rejetée → au moins une moyenne est significativement différente des autres moyennes.
# *6. Test post-hoc de Tukey*
    * Comparaisons significatives :
        * Allemagne vs France
        * Autriche vs France
        * Belgique vs France
  ❌ Pas de différence significative entre Allemagne, Autriche et Belgique.
# *✅ Conclusion*
    * Les timbres français ont une épaisseur significativement différente (et plus faible) que ceux des autres pays. Cela confirme l’intuition de Rémi.
