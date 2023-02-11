file:: [System_Design_Interview_An_Insider’s_Guide_(Alex_Xu)_1668886834673_0.pdf](../assets/System_Design_Interview_An_Insider’s_Guide_(Alex_Xu)_1668886834673_0.pdf)
file-path:: ../assets/System_Design_Interview_An_Insider’s_Guide_(Alex_Xu)_1668886834673_0.pdf

- Single server setup
  ls-type:: annotation
  hl-page:: 6
  hl-color:: yellow
  id:: 63794612-269f-4ca0-bb69-50ed933acdcd
- [:span]
  ls-type:: annotation
  hl-page:: 6
  hl-color:: yellow
  id:: 637946af-b6f6-4d56-aa77-013dd4fc902c
  hl-type:: area
  hl-stamp:: 1668892335356
- Database
  ls-type:: annotation
  hl-page:: 8
  hl-color:: yellow
  id:: 63794b3e-542c-4971-aa58-47607d328ed0
- [:span]
  ls-type:: annotation
  hl-page:: 8
  hl-color:: yellow
  id:: 63794f0b-476b-411d-9594-994dafea70de
  hl-type:: area
  hl-stamp:: 1668894475023
- Vertical scaling vs horizontal scaling
  ls-type:: annotation
  hl-page:: 9
  hl-color:: yellow
  id:: 63794f26-d984-4a03-a114-0ebe80ce6d45
- Load balancer
  ls-type:: annotation
  hl-page:: 10
  hl-color:: yellow
  id:: 6379518e-15c4-4546-96e8-0f504f10081a
- [:span]
  ls-type:: annotation
  hl-page:: 10
  hl-color:: yellow
  id:: 637951e0-ccf8-4fad-bfa2-37b56af53019
  hl-type:: area
  hl-stamp:: 1668895199791
- Database replication
  ls-type:: annotation
  hl-page:: 12
  hl-color:: yellow
  id:: 63795db8-2f7d-4dce-a46d-95f17f74b0fa
- [:span]
  ls-type:: annotation
  hl-page:: 12
  hl-color:: yellow
  id:: 63795dc9-ad18-4142-89d8-05c6813bbeb6
  hl-type:: area
  hl-stamp:: 1668898249143
- Cache
  ls-type:: annotation
  hl-page:: 15
  hl-color:: yellow
  id:: 63796475-8b57-46d0-ab59-3efeb3c6ca01
- [:span]
  ls-type:: annotation
  hl-page:: 15
  hl-color:: blue
  id:: 638ccb4e-3b02-4423-ba34-ed509bfdf26b
  hl-type:: area
  hl-stamp:: 1670171468112
- Content delivery network (CDN)
  ls-type:: annotation
  hl-page:: 17
  hl-color:: blue
  id:: 638cd160-0923-46b8-b6ed-4f5da5089977
- enables the caching of HTML pages that are based on request path, query strings, cookies, and request header
  ls-type:: annotation
  hl-page:: 17
  hl-color:: blue
  id:: 638cd859-1f62-4ee0-bb44-9f467a32ce59
- Figure 1-10 demonstrates the CDN workflow.
  ls-type:: annotation
  hl-page:: 17
  hl-color:: blue
  id:: 638ce61e-6d75-4dd8-b3ce-ff753df0bab1
- Here is how CDN works at the high-level: when a user visits a website, a CDN server closest to the user will deliver static content. Intuitively, the further users are from CDN servers, the slower the website loads.
  ls-type:: annotation
  hl-page:: 17
  hl-color:: green
  id:: 638ce639-2526-42f2-967e-5ca131489f7b
  hl-stamp:: 1670178366683
- [:span]
  ls-type:: annotation
  hl-page:: 17
  hl-color:: yellow
  id:: 638ce64f-ba44-417e-8cfb-9460e92e59ce
  hl-type:: area
  hl-stamp:: 1670178380833
- Cos
  ls-type:: annotation
  hl-page:: 18
  hl-color:: green
  id:: 638ce6bb-fd55-461b-9468-a0387c970b11
  hl-stamp:: 1670178674122
- Setting an appropriate cache expir
  ls-type:: annotation
  hl-page:: 18
  hl-color:: red
  id:: 638ce6c1-afb8-43ed-bb27-a0a5a477c155
  hl-stamp:: 1670178651522
- CDN fallback
  ls-type:: annotation
  hl-page:: 18
  hl-color:: green
  id:: 638ce6c5-62e1-4362-8a9d-ced59ad2d896
  hl-stamp:: 1670178691453
- Invalidating files:
  ls-type:: annotation
  hl-page:: 18
  hl-color:: purple
  id:: 638ce6c8-141a-4eca-aa41-098705955ade
  hl-stamp:: 1670178702458
- CDNs are run by third-party providers, and you are charged for data transfers in and out of the CDN
  ls-type:: annotation
  hl-page:: 18
  hl-color:: green
  id:: 638ce6ff-422f-4e60-b0ce-36a0befc5568
  hl-stamp:: 1670178565658
- g infrequently used assets provides no significant benefits so you should consider moving them out of the CDN.
  ls-type:: annotation
  hl-page:: 18
  hl-color:: purple
  id:: 638ce710-8a6b-4262-b57d-8337265b8dcb
  hl-stamp:: 1670178655858
- If it is too long, the content might no longer be fresh.
  ls-type:: annotation
  hl-page:: 18
  hl-color:: red
  id:: 638ce72f-9ea5-412e-92f9-50b499ad7a01
- If it is too short, it can cause repeat reloading of content from origin servers to the CDN.
  ls-type:: annotation
  hl-page:: 18
  hl-color:: purple
  id:: 638ce731-00f6-40b7-a3bd-ab94109878a3
  hl-stamp:: 1670178687298
- If there is a temporary CDN outage, clients should be able to detect the problem and request resources from the origin.
  ls-type:: annotation
  hl-page:: 18
  hl-color:: green
  id:: 638ce743-d83a-471f-b9a2-00d6e0e261da
  hl-stamp:: 1670178693707
- emove a file from the CDN before it expires
  ls-type:: annotation
  hl-page:: 18
  hl-color:: purple
  id:: 638ce7a4-f92e-4e26-afa2-045f573a4115
- Invalidate the CDN object using APIs provided by CDN vendors.
  ls-type:: annotation
  hl-page:: 18
  hl-color:: red
  id:: 638ce7b0-5654-4d92-a7b3-21838aa9b9a5
  hl-stamp:: 1670178740890
- Use object versioning to serve a different version of the object. 
  ls-type:: annotation
  hl-page:: 18
  hl-color:: yellow
  id:: 638ce7bc-71a2-4705-b9fc-549f22410db3
  hl-stamp:: 1670178750818
- version number 2 is added to the query string: image.png?v=2.
  ls-type:: annotation
  hl-page:: 18
  hl-color:: yellow
  id:: 638ce7cb-b3e3-4858-bc77-2b8bd5d8fb20
- [:span]
  ls-type:: annotation
  hl-page:: 19
  hl-color:: yellow
  id:: 638ce7e0-eea8-4079-82ef-6d1fbd30ff89
  hl-type:: area
  hl-stamp:: 1670178783978
- Stateless web tier
  ls-type:: annotation
  hl-page:: 20
  hl-color:: yellow
  id:: 638ce800-bc22-4593-84dd-267316e75c6a
- A stateful server remembers client data (state) from one request to the next
  ls-type:: annotation
  hl-page:: 20
  hl-color:: yellow
  id:: 638cfd66-8d79-4e12-bc2e-ea281822db92
- server keeps no state information.
  ls-type:: annotation
  hl-page:: 20
  hl-color:: yellow
  id:: 638cfd88-06f0-4f99-a1c4-77c8cdafeacb
- Figure 1-12 shows an example of a stateful architecture.
  ls-type:: annotation
  hl-page:: 20
  hl-color:: yellow
  id:: 638cfd92-2d6e-4ff3-9d82-b6a82de0937b
- which fetch state data from a shared data store. State data is stored in a shared data store and kept out of web servers.
  ls-type:: annotation
  hl-page:: 21
  hl-color:: yellow
  id:: 638cfe5c-ba81-46a4-940a-9efcb19de683
- [:span]
  ls-type:: annotation
  hl-page:: 22
  hl-color:: yellow
  id:: 638cfe91-53ed-49ef-9949-02a281ea5eaf
  hl-type:: area
  hl-stamp:: 1670184593236
- Data centers
  ls-type:: annotation
  hl-page:: 23
  hl-color:: yellow
  id:: 638cff33-b0f4-4455-82fa-ed1bfa9fed4f