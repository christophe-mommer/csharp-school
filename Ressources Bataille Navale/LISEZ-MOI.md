# Ressources du TP bataille navale

Ces ressources accompagnent « Cours C# ASP.NET - Bataille Navale - autonomie.pptx ».

Le socle est votre point de départ. Avec l’IA, explorez les pistes du backlog et proposez un périmètre ambitieux et cohérent. Vous êtes responsables des fonctionnalités choisies, de leur qualité et de leur maîtrise. L’ambition, la pertinence et la finition du périmètre réalisé sont évaluées. Les arbitrages et les renoncements doivent être défendables à partir des faits du projet.

Copiez global.json à la racine du dépôt avant les commandes de création de la solution. Il sélectionne un SDK .NET 10 stable installé ; il n’installe pas le SDK. Vérifiez `dotnet --version`. Les vérifications de cette relecture utilisent le SDK 10.0.401.

Copiez les gabarits de livrables et complétez le contexte du projet. Utilisez vos échanges, décisions et observations réels. PROMPTS.md retrace les échanges décisifs, les ADR les choix structurants et REVUE-IA.md vos trois revues argumentées minimum. Des liens entre ces documents évitent de dupliquer les analyses.

## Exemples génériques

Le référentiel présente les mécanismes de C#, ASP.NET Core, Blazor et gRPC sur un catalogue de produits. Les extraits correspondent à des contextes distincts : fichier C#, Program.cs, composant Razor ou contrat Protobuf. Ils ne constituent pas une application complète à copier. Vous concevez les contrats et l’implémentation de la bataille navale.

- `Referentiel.md` reprend les diapositives du référentiel et leurs extraits.
- `Exemples/ContratsExemples.cs.txt` définit les types génériques et la règle de prix utilisée pour illustrer xUnit.
- `Exemples/catalogue.proto` définit un échange gRPC de démonstration.
- `Exemples/CatalogueGrpcService.cs.txt` illustre une réponse et une validation ; enregistrez le validateur comme indiqué diapo 51.
- `api.http` illustre des requêtes sur le catalogue : adaptez l’adresse à votre serveur de démonstration. Construisez les requêtes du jeu à partir de vos propres contrats.

Les noms Catalogue.API et Catalogue.App désignent les projets de démonstration. Adaptez les commandes au projet dans lequel vous explorez le mécanisme. Configurez les origines, l’hébergement et les échanges navigateur selon votre environnement et la documentation de référence.

## Sources techniques

Le cycle de vie des composants est décrit dans la [documentation Blazor](https://learn.microsoft.com/en-us/aspnet/core/blazor/components/lifecycle?view=aspnetcore-10.0). La configuration navigateur est détaillée dans la [documentation gRPC-Web](https://learn.microsoft.com/en-us/aspnet/core/grpc/grpcweb?view=aspnetcore-10.0) et la [documentation CORS](https://learn.microsoft.com/en-us/aspnet/core/security/cors?view=aspnetcore-10.0). L’appel explicite aux validateurs est décrit dans la [documentation FluentValidation](https://docs.fluentvalidation.net/en/latest/aspnet.html).
