```mermaid
flowchart TB
  subgraph UnRaid;

    subgraph disks and shares
      mnt-->cache & cache_app & disk1 & disk2 & disk3 & disk4 & disk5 & disk6 & disk7 & disk8;
      cache:::ssd -->downloads & code;
      cache_app:::nvme -->appdata & domains & isos & system;
      disk1:::hdd -->audiobooks & backup & code & downloads & ebooks & films & music & podcasts & popvids & private & restore & tvshows
      disk2:::hdd -->audiobooks & backup & code & downloads & ebooks & films & music & podcasts & popvids & private & restore & tvshows
      disk3:::hdd -->audiobooks & backup & code & downloads & ebooks & films & music & podcasts & popvids & private & restore & tvshows
      disk4:::hdd -->audiobooks & backup & code & downloads & ebooks & films & music & podcasts & popvids & private & restore & tvshows
      disk5:::hdd -->audiobooks & backup & code & downloads & ebooks & films & music & podcasts & popvids & private & restore & tvshows
      disk6:::hdd -->audiobooks & backup & code & downloads & ebooks & films & music & podcasts & popvids & private & restore & tvshows
      disk7:::hdd -->audiobooks & backup & code & downloads & ebooks & films & music & podcasts & popvids & private & restore & tvshows
      disk8:::hdd -->audiobooks & backup & code & downloads & ebooks & films & music & podcasts & popvids & private & restore & tvshows
    end    

    subgraph Key;
      ssd:::ssd;
      nvme:::nvme;
      hdd:::hdd;
      share:::share;
    end
    
    classDef ssd fill:#f96;
    classDef nvme fill:#996;
    classDef hdd fill:#696;
    classDef hdd share:#396;
    
  end
```

|    Share   |                         Usage                        |
|------------|------------------------------------------------------|
| appdata    | Docker persistent stotrage                           |
| audiobooks | CD rips                                              |
| backup     | a few temp backup jobs dump their output here        |
| code       | a few small coding projects                          |
| domains    | VM images                                            |
| downloads  | temporary home for downloads                         |
| ebooks     | purchased audiobooks                                 |
| films      | DVD/Bluray rips                                      |
| isos       | ISO images used for VM's                             |
| music      | CD rips                                              |
| podcasts   | a few favourite podcasts live here for easy locating |
| popvids    | DVD rips                                             |
| private    | personal stuff                                       |
| restore    | temporary home for restroing backups                 |
| system     | Docker images, containers, volumes                   |
| tvshows    | DVD/Bluray rips                                      |
