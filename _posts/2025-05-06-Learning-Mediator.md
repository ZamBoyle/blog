---
layout: post
title:  "Mediator en .NET"
date:   2025-05-05 14:58:36 +0200
categories: .NET, C#
---
Qu'est-ce que Mediator ?

Voici un exemple de code qui illustre le modèle Mediator en C#.

```csharp
services.AddMediatR(cfg => {
    cfg.RegisterServicesFromAssembly(typeof(Startup).Assembly);
    cfg.AddBehavior<PingPongBehavior>();
    cfg.AddStreamBehavior<PingPongStreamBehavior>();
    cfg.AddRequestPreProcessor<PingPreProcessor>();
    cfg.AddRequestPostProcessor<PingPongPostProcessor>();
    cfg.AddOpenBehavior(typeof(GenericBehavior<,>));
    });
```

