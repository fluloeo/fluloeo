## Всем привет! 
flowchart LR

    %% ===== SKY =====

    star1["✦"]
    star2["✧"]
    moon["◐"]
    star3["✦"]
    star4["·"]

    star1 ~~~ star2 ~~~ moon ~~~ star3 ~~~ star4


    %% ===== MOUNTAINS =====

    mt1["╱╲"]
    mt2["╱  ╲"]
    mt3["╱╲"]
    mt4["╱    ╲"]
    mt5["╱╲"]
    mt6["╱  ╲"]
    mt7["╱╲"]

    mt1 --- mt2 --- mt3 --- mt4 --- mt5 --- mt6 --- mt7


    %% ===== FOREST =====

    t1["🌲"]
    t2["🌲"]
    t3["🌲"]
    t4["🌲"]
    t5["🌲"]
    t6["🌲"]
    t7["🌲"]
    t8["🌲"]
    t9["🌲"]
    t10["🌲"]
    t11["🌲"]

    t1 ~~~ t2 ~~~ t3 ~~~ t4 ~~~ t5 ~~~ t6 ~~~ t7 ~~~ t8 ~~~ t9 ~~~ t10 ~~~ t11


    %% ===== CABIN =====

    treeL["🌲"]
    cabin["🏚️"]
    treeR["🌲"]

    treeL ~~~ cabin ~~~ treeR


    %% ===== RIVER =====

    r1["〰"]
    r2["〰"]
    r3["〰"]
    r4["〰"]
    r5["〰"]
    r6["〰"]
    r7["〰"]

    r1 ~~~ r2 ~~~ r3 ~~~ r4 ~~~ r5 ~~~ r6 ~~~ r7


    %% ===== FRONT FOREST =====

    f1["🌲"]
    f2["🌲"]
    f3["🌲"]
    f4["🌲"]
    f5["🌲"]
    f6["🌲"]
    f7["🌲"]
    f8["🌲"]
    f9["🌲"]

    f1 ~~~ f2 ~~~ f3 ~~~ f4 ~~~ f5 ~~~ f6 ~~~ f7 ~~~ f8 ~~~ f9


    %% ===== VERTICAL ALIGNMENT =====

    star1 ~~~ mt1
    star2 ~~~ mt2
    moon ~~~ mt4
    star3 ~~~ mt6

    mt1 ~~~ t1
    mt2 ~~~ t2
    mt3 ~~~ t3
    mt4 ~~~ t4
    mt5 ~~~ t5
    mt6 ~~~ t6
    mt7 ~~~ t7

    t4 ~~~ cabin
    t5 ~~~ cabin
    t6 ~~~ cabin

    cabin ~~~ r4

    r1 ~~~ f1
    r2 ~~~ f2
    r3 ~~~ f3
    r4 ~~~ f4
    r5 ~~~ f5
    r6 ~~~ f6
    r7 ~~~ f7


    %% ===== STYLE =====

    classDef moon fill:#171326,stroke:#c4b5fd,color:#f5f3ff,stroke-width:3px;
    classDef star fill:#0b1020,stroke:#0b1020,color:#e9d5ff;
    classDef mountain fill:#1b2435,stroke:#64748b,color:#cbd5e1,stroke-width:2px;
    classDef tree fill:#10251d,stroke:#315c49,color:#d1fae5,stroke-width:2px;
    classDef cabin fill:#2a1b14,stroke:#b78b62,color:#ffe7c2,stroke-width:3px;
    classDef river fill:#101827,stroke:#456781,color:#bfdbfe;

    class moon moon;
    class star1,star2,star3,star4 star;
    class mt1,mt2,mt3,mt4,mt5,mt6,mt7 mountain;
    class t1,t2,t3,t4,t5,t6,t7,t8,t9,t10,t11 tree;
    class treeL,treeR,f1,f2,f3,f4,f5,f6,f7,f8,f9 tree;
    class cabin cabin;
    class r1,r2,r3,r4,r5,r6,r7 river;


    %% hide layout edges

    linkStyle default stroke:transparent,stroke-width:0px;

    %% mountain outline edges visible

    linkStyle 5,6,7,8,9,10 stroke:#64748b,stroke-width:2px;
