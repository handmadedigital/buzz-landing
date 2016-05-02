<script>
  export default {
    name: "Home",

    ready: function() {

      var controller = new ScrollMagic.Controller(),
          kart1SceneTl = new TimelineLite(),
          kart2SceneTl = new TimelineLite(),
          kart3SceneTl = new TimelineLite(),
          blueCarSceneTl = new TimelineLite(),
          treePopOut = new TimelineLite(),
          firstScene = document.getElementById('first-section'),
          firstSceneWidth = firstScene.scrollWidth,
          firstSceneDuration = (firstSceneWidth/1920) * 600;

      var blueCar = document.getElementById('blue-car'),
          building = document.getElementById('building'),
          coffeeHouse = document.getElementById('coffee-house'),
          crossSign1 = document.getElementById('cross-sign-1'),
          crossSign2 = document.getElementById('cross-sign-2'),
          golfKart1 = document.getElementById('golf-kart-1'),
          golfKart2 = document.getElementById('golf-kart-2'),
          golfKart3 = document.getElementById('golf-kart-3'),
          greekBuilding = document.getElementById('greek-building'),
          house1 = document.getElementById('house-1'),
          house2 = document.getElementById('house-2'),
          house3 = document.getElementById('house-3'),
          storeBuilding = document.getElementById('store-building'),
          tent = document.getElementById('tent'),
          tentCar = document.getElementById('tent-car'),
          tentTree = document.getElementById('tent-tree'),
          tree1 = document.getElementById('tree-1'),
          tree2 = document.getElementById('tree-2'),
          tree3 = document.getElementById('tree-3'),
          tree4 = document.getElementById('tree-4'),
          tree5 = document.getElementById('tree-5'),
          tree6 = document.getElementById('tree-6'),
          tree7 = document.getElementById('tree-7'),
          tree8 = document.getElementById('tree-8'),
          tree9 = document.getElementById('tree-9'),
          ourGoals = document.getElementById('our-goals'),
          daytimeHours = document.getElementById('daytime-hours'),
          eveningHours = document.getElementById('evening-hours'),
          socialResponsibility = document.getElementById('social-responsibility'),
          weDontStopThere = document.getElementById('we-dont-stop-there');

        var tree1PopIn = new ScrollMagic.Scene({
          triggerElement: tree1,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree1, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tree2PopIn = new ScrollMagic.Scene({
          triggerElement: tree2,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree2, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tree3PopIn = new ScrollMagic.Scene({
          triggerElement: tree3,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree3, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tree4PopIn = new ScrollMagic.Scene({
          triggerElement: tree4,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree4, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tree5PopIn = new ScrollMagic.Scene({
          triggerElement: tree5,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree5, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tree6PopIn = new ScrollMagic.Scene({
          triggerElement: tree6,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree6, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tree7PopIn = new ScrollMagic.Scene({
          triggerElement: tree7,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree7, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tree8PopIn = new ScrollMagic.Scene({
          triggerElement: tree8,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree8, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tree9PopIn = new ScrollMagic.Scene({
          triggerElement: tree9,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tree9, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var house1PopIn = new ScrollMagic.Scene({
          triggerElement: house1,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(house1, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var house2PopIn = new ScrollMagic.Scene({
          triggerElement: house2,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(house2, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var house3PopIn = new ScrollMagic.Scene({
          triggerElement: house3,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(house3, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tentPopIn = new ScrollMagic.Scene({
          triggerElement: tent,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tent, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tentCarPopIn = new ScrollMagic.Scene({
          triggerElement: tentCar,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tentCar, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var tentTreePopIn = new ScrollMagic.Scene({
          triggerElement: tentTree,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(tentTree, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var coffeeHousePopIn = new ScrollMagic.Scene({
          triggerElement: coffeeHouse,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(coffeeHouse, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var buildingPopIn = new ScrollMagic.Scene({
          triggerElement: building,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(building, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var greekBuildingPopIn = new ScrollMagic.Scene({
          triggerElement: greekBuilding,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(greekBuilding, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var crossSign1PopIn = new ScrollMagic.Scene({
          triggerElement: crossSign1,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(crossSign1, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var crossSign2PopIn = new ScrollMagic.Scene({
          triggerElement: crossSign2,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(crossSign2, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var storeBuildingPopIn = new ScrollMagic.Scene({
          triggerElement: storeBuilding,
          triggerHook: 'onEnter',
          offset: 100,
        }).setTween(TweenMax.from(storeBuilding, 1.4, {
          scaleY: 0,
          transformOrigin:"0% 100%",
          ease: Elastic.easeOut
        })).addTo(controller);

        var ourGoalsSlideIn= new ScrollMagic.Scene({
          triggerElement: ourGoals,
          triggerHook: 'onEnter',
          offset: 100
        }).setTween(TweenMax.from(ourGoals, 2, {
          x: 1400,
          opacity: 0,
          transformOrigin:"0% 100%",
          ease: Power2.easeOut
        })).addTo(controller);

        var daytimeHoursSlideIn= new ScrollMagic.Scene({
          triggerElement: daytimeHours,
          triggerHook: 'onEnter',
          offset: 100
        }).setTween(TweenMax.from(daytimeHours, 2, {
          x: -1400,
          opacity: 0,
          transformOrigin:"0% 100%",
          ease: Power2.easeOut
        })).addTo(controller);

        var eveningHoursSlideIn= new ScrollMagic.Scene({
          triggerElement: eveningHours,
          triggerHook: 'onEnter',
          offset: 100
        }).setTween(TweenMax.from(eveningHours, 2, {
          x: 1400,
          opacity: 0,
          transformOrigin:"0% 100%",
          ease: Power2.easeOut
        })).addTo(controller);

        var socialResponsibilitySlideIn= new ScrollMagic.Scene({
          triggerElement: socialResponsibility,
          triggerHook: 'onEnter',
          offset: 100
        }).setTween(TweenMax.from(socialResponsibility, 2, {
          x: -1400,
          opacity: 0,
          transformOrigin:"0% 100%",
          ease: Power2.easeOut
        })).addTo(controller);

        var weDontStopThereSlideIn= new ScrollMagic.Scene({
          triggerElement: weDontStopThere,
          triggerHook: 'onEnter',
          offset: 100
        }).setTween(TweenMax.from(weDontStopThere, 2, {
          x: 1400,
          opacity: 0,
          transformOrigin:"0% 100%",
          ease: Power2.easeOut
        })).addTo(controller);






      console.log(firstSceneDuration + " " + firstSceneWidth);

      kart1SceneTl
      .to("#golf-kart-1", 6, {x:-750, y:440, ease: Power2.easeOut})
      .to("#passanger-1", 1, {x:40, y: 20, ease: Power2.ease})
      .to("#passanger-1", 0.1, {opacity:0, ease: Power2.ease})
      .to("#golf-kart-1", 8, {x:-1500, y:880, ease: Power2.ease});

      kart2SceneTl
      .to(golfKart2, 6, {x:1400, y:820, ease: Power2.easeOut});

      kart3SceneTl
      .to(golfKart3, 6, {x:370, y:210, ease: Power2.easeOut});




      var kart1Scene = new ScrollMagic.Scene({
        triggerElement: '#first-section',
        triggerHook: 'onLeave',
        duration: firstSceneDuration
      }).setTween(kart1SceneTl).addTo(controller);

      var kart2Scene = new ScrollMagic.Scene({
        triggerElement: daytimeHours,
        triggerHook: 'onLeave',
        duration: 1200
      }).setTween(kart2SceneTl).addTo(controller);

      var kart3Scene = new ScrollMagic.Scene({
        triggerElement: weDontStopThere,
        offset: 200,
        duration: 400
      }).setTween(kart3SceneTl).addTo(controller);

    },

    methods: {
      strech: function(id) {
        TweenMax.to('#'+id, 0.2, { scaleY:1.1, y:-10});
        TweenMax.to('#'+id, 0.2, { scaleY:1,y:0, delay: 0.2});
        console.log(id);
      },
      moveKart: function() {
        TweenMax.to("#golf-kart-1", 6, {x:-750, y:440, ease: Power2.easeOut});
        TweenMax.to("#human-1", 2, {x:80, y:50, delay:6, ease: Power2.ease});
        TweenMax.to("#human-1", 0.2, {
          scaleY: 1.1,
          delay:5.8,
          yoyo:true,
          repeat:-1,
          ease: Power2.ease//,
          //onCompleteParams:[elementItem],
          //onComplete: elementMoveUp
        });
        TweenMax.to("#human-1", 0.1, {opacity:0, delay:8, ease: Power2.ease});
        TweenMax.to("#golf-kart-1", 8, {x:-1500, y:880, delay:8, ease: Power2.ease});
      }
    }
  }
</script>

<template>
  <svg id="first-section" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 1916.5 4100.5">
    <style>
      .st0{fill:#BCBCBC;} .st1{opacity:0.2;fill:#0E1D26;} .st2{fill:#979797;} .st3{fill:#CCCBCB;} .st4{fill:#11A4B1;} .st5{fill:#5987A1;} .st6{fill:#70A6CB;} .st7{fill:#C57267;} .st8{fill:#E77F6E;} .st9{opacity:0.5;fill:#08324A;} .st10{fill:#373636;} .st11{fill:#FFFFFF;} .st12{fill:#CEEAF9;} .st13{fill:#274550;} .st14{enable-background:new ;} .st15{fill:none;} .st16{opacity:0.2;fill:#0A324A;} .st17{fill:#774927;} .st18{fill:#74B358;} .st19{fill:#91CA6D;} .st20{fill:#70A7CD;} .st21{fill:#5988A3;} .st22{fill:#175079;} .st23{fill:#0D3A56;} .st24{fill:#052738;} .st25{fill:#296F9B;} .st26{fill:#1E76AE;} .st27{fill:#E9EEE3;} .st28{fill:#5892CE;} .st29{fill:#E7806F;} .st30{fill:#C16B60;} .st31{fill:#E6F5F9;} .st32{fill:#BF6559;} .st33{fill:#A35C56;} .st34{fill:#CC766A;} .st35{fill:#BC6C64;} .st36{fill:#90C4E2;} .st37{fill:#C1685F;} .st38{fill:#D87668;} .st39{opacity:0.6;} .st40{fill:#08324A;} .st41{fill:#833C2D;} .st42{fill:#D17546;} .st43{fill:#B05538;} .st44{opacity:0.3;} .st45{fill:#0D2025;} .st46{fill:#E9E2DA;} .st47{fill:#427896;} .st48{fill:#D1BA87;} .st49{fill:#FEE5A4;} .st50{fill:#BA9458;} .st51{fill:#4B8095;} .st52{fill:#3E5C69;} .st53{fill:#887552;} .st54{opacity:0.4;} .st55{fill:#4C3368;} .st56{fill:#3E6677;} .st57{fill:#DBBC82;} .st58{opacity:0.8;} .st59{fill:#362C2E;} .st60{fill:#683A16;} .st61{fill:#3F2511;} .st62{fill:#E0B073;} .st63{fill:#DDB193;} .st64{fill:#41718C;} .st65{fill:#633293;} .st66{fill:#5188A0;} .st67{fill:#939598;} .st68{fill:#576A78;} .st69{fill:#6BB29F;} .st70{fill:#8BD1CA;} .st71{fill:#F9A86B;} .st72{fill:#DE625B;} .st73{fill:#203D62;} .st74{fill:#3F2E1C;} .st75{fill:#6E5649;} .st76{fill:#BB6429;} .st77{fill:#F68A58;} .st78{fill:#112A44;} .st79{fill:#6D2814;} .st80{fill:#FCC084;} .st81{fill:#9C492A;} .st82{fill:#BF3B37;} .st83{fill:#655959;} .st84{fill:#2E2119;} .st85{fill:#413123;} .st86{fill:#E4EEF9;} .st87{fill:#CCDDEE;} .st88{fill:#3D4A67;} .st89{fill:#94CB6F;} .st90{font-family:&apos;OpenSans-BoldItalic&apos;;} .st91{font-size:52px;} .st92{fill:#010101;} .st93{font-family:&apos;OpenSans-Light&apos;;} .st94{font-size:20.3984px;} .st95{fill:#EB6126;} .st96{fill:#A8B4C9;} .st97{fill:#A7C7CB;} .st98{fill:#B4D3D9;} .st99{fill:#93AFB4;} .st100{fill:#F3B727;} .st101{fill:#27AFC6;} .st102{fill:#68AEC4;} .st103{fill:#5B9AAD;} .st104{fill:#E5B73D;} .st105{fill:#BBC359;} .st106{fill:#AFB849;} .st107{fill:#9FA838;} .st108{fill:#DFE4EF;} .st109{fill:#A5AC3F;} .st110{fill:#60A5BC;} .st111{fill:#4B576A;} .st112{fill:#A6AD51;} .st113{fill:#5793A8;} .st114{fill:#A5B139;} .st115{fill:#234A59;} .st116{fill:#F8FAFD;} .st117{fill:#D2EAF9;} .st118{fill:#F3EFE4;} .st119{fill:#E4EAEC;} .st120{fill:#B8C351;} .st121{fill:#E0CEA7;} .st122{fill:#D7D3CA;} .st123{fill:#ECE8E0;} .st124{fill:#1E96BF;} .st125{opacity:0.7;fill:#27AFC6;} .st126{fill:#FED7AF;} .st127{fill:#F5CDA5;} .st128{fill:#FFD9AF;} .st129{fill:#FFE1B9;} .st130{fill:#195B6F;} .st131{fill:#206579;} .st132{fill:#969696;} .st133{fill:#FFC934;} .st134{fill:#1E3241;} .st135{fill:#293D4B;} .st136{fill:#FFDC48;} .st137{fill:#BABCBA;} .st138{fill:#EE6E23;} .st139{fill:#314E67;} .st140{fill:#FCB039;} .st141{fill:#DCEFF4;} .st142{fill:#FED098;} .st143{fill:#E0A86A;} .st144{fill:#B5DCE6;} .st145{fill:#080C0E;} .st146{fill:#D2985D;} .st147{fill:#F26428;} .st148{fill:#BB3426;} .st149{fill:#3A2210;} .st150{fill:#353635;} .st151{fill:#939393;} .st152{fill:#735147;} .st153{fill:#181818;} .st154{fill:#E2E2E2;} .st155{fill:#8A6D63;} .st156{fill:#E05926;} .st157{fill:#3A1311;} .st158{fill:#593416;} .st159{fill:#333333;} .st160{fill:#0999A0;} .st161{fill:#428E78;} .st162{fill:#F15A2B;} .st163{fill:#9B201F;} .st164{font-size:36.2851px;} .st165{font-size:20.4px;} .st166{clip-path:url(#SVGID_2_);} .st167{fill:#8C6A45;} .st168{fill:#DC9B45;} .st169{fill:#EFC992;} .st170{fill:#DBB27D;} .st171{fill:#F5CC90;} .st172{fill:#FFDDA4;} .st173{fill:#DAB177;} .st174{fill:#F2F1F0;} .st175{fill:#EA8854;} .st176{fill:#5A5A5A;} .st177{fill:#2E2E2C;} .st178{font-size:20.264px;} .st179{clip-path:url(#SVGID_4_);} .st180{clip-path:url(#SVGID_6_);} .st181{fill:#9E8B43;} .st182{opacity:0.2;fill:#1A242F;} .st183{fill:#6A6032;} .st184{fill:#76593D;} .st185{fill:#8C724E;} .st186{fill:#CFA873;} .st187{clip-path:url(#SVGID_8_);} .st188{fill:#C8B69C;} .st189{fill:#2A343F;} .st190{fill:#AFDCEF;} .st191{fill:#8F191C;} .st192{opacity:0.34;fill:#FFFFFF;} .st193{fill:#766553;} .st194{fill:#8B5D29;} .st195{opacity:0.41;fill:#1A242F;} .st196{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;} .st197{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:16.5747,16.5747;} .st198{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:15.9934,15.9934;} .st199{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:17.1563,17.1563;} .st200{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:15.2018,15.2018;} .st201{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:16.079,16.079;} .st202{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:14.3915,14.3915;} .st203{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:15.8439,15.8439;} .st204{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:16.0193,16.0193;} .st205{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:15.8032,15.8032;} .st206{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:16.0617,16.0617;} .st207{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:16.1473,16.1473;} .st208{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:16.0536,16.0536;} .st209{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:16.3102,16.3102;} .st210{fill:none;stroke:#FFFFFF;stroke-width:4;stroke-miterlimit:10;stroke-dasharray:19.8867,19.8867;} .st211{fill:#272626;} .st212{fill:#BBBBBB;} .st213{fill:#676767;} .st214{fill:#1A1A1A;} .st215{fill:#BF2026;} .st216{fill:#E32526;} .st217{fill:#818181;} .st218{fill:#919191;} .st219{fill:#4C4A45;} .st220{fill:#66635F;} .st221{fill:#1F1D1B;} .st222{fill:#353330;} .st223{fill:#4E4E4E;} .st224{fill:#4A4949;} .st225{fill:#4B4B4B;} .st226{fill:#85827C;} .st227{fill:#7A7873;} .st228{fill:#D02027;} .st229{fill:#0C0C0C;} .st230{fill:url(#SVGID_9_);} .st231{fill:#193138;} .st232{fill:#CBEBF7;} .st233{fill:#5E5E5E;} .st234{fill:#4A707F;} .st235{fill:#D1ECFA;} .st236{fill:#F8A8A2;} .st237{fill:#C97165;} .st238{fill:#426B7D;} .st239{fill:#F3B7AE;} .st240{fill:#E0DEDE;} .st241{fill:url(#SVGID_10_);} .st242{fill:url(#SVGID_11_);} .st243{opacity:0.5;fill:#0A324A;} .st244{fill:#FED193;} .st245{fill:#DCB37E;} .st246{fill:#B6D7E2;} .st247{fill:#D1E8F4;} .st248{fill:#9FDCF1;} .st249{fill:#5284A0;} .st250{opacity:0.61;} .st251{fill:#515151;} .st252{fill:#3A3A39;} .st253{fill:#797979;} .st254{fill:#665147;} .st255{fill:#444444;} .st256{font-size:20.1068px;} .st257{fill:#C7C6C6;} .st258{fill:#ABABAB;} .st259{fill:#78AA96;} .st260{fill:#0E5165;} .st261{fill:#B5B5B5;} .st262{fill:#DDDDDC;} .st263{fill:#C8C8C8;} .st264{fill:#EFB354;} .st265{fill:#F15D47;} .st266{fill:#404050;} .st267{fill:#4A4A63;} .st268{fill:#757694;} .st269{fill:#DDDCE8;} .st270{fill:#DD4541;} .st271{fill-rule:evenodd;clip-rule:evenodd;fill:#C1DDD4;} .st272{fill-rule:evenodd;clip-rule:evenodd;fill:#9CBCAD;} .st273{fill-rule:evenodd;clip-rule:evenodd;fill:#AEC8BD;} .st274{fill:#424040;} .st275{fill-rule:evenodd;clip-rule:evenodd;fill:#623822;} .st276{fill-rule:evenodd;clip-rule:evenodd;fill:#452616;} .st277{fill-rule:evenodd;clip-rule:evenodd;fill:#D15F2D;} .st278{fill-rule:evenodd;clip-rule:evenodd;fill:#B14725;} .st279{fill-rule:evenodd;clip-rule:evenodd;fill:#85391C;} .st280{fill-rule:evenodd;clip-rule:evenodd;fill:#E37949;} .st281{fill-rule:evenodd;clip-rule:evenodd;fill:#EEE4D3;} .st282{fill-rule:evenodd;clip-rule:evenodd;fill:#A39D9A;} .st283{fill-rule:evenodd;clip-rule:evenodd;fill:#FFFFFF;} .st284{fill-rule:evenodd;clip-rule:evenodd;fill:#301D13;} .st285{fill-rule:evenodd;clip-rule:evenodd;fill:#724129;} .st286{fill-rule:evenodd;clip-rule:evenodd;fill:#5D5856;} .st287{fill-rule:evenodd;clip-rule:evenodd;fill:#6B5E5E;} .st288{fill-rule:evenodd;clip-rule:evenodd;fill:#F4D596;} .st289{fill-rule:evenodd;clip-rule:evenodd;fill:#A5978F;} .st290{fill:#4A686B;} .st291{fill:#6DA1A1;} .st292{fill-rule:evenodd;clip-rule:evenodd;fill:#527275;} .st293{fill-rule:evenodd;clip-rule:evenodd;fill:#9C9C9D;} .st294{fill-rule:evenodd;clip-rule:evenodd;fill:#6A6A6A;} .st295{fill-rule:evenodd;clip-rule:evenodd;fill:#364444;} .st296{fill-rule:evenodd;clip-rule:evenodd;fill:#89BBBE;} .st297{fill-rule:evenodd;clip-rule:evenodd;fill:#ABABAB;} .st298{fill-rule:evenodd;clip-rule:evenodd;fill:#6D6966;} .st299{fill-rule:evenodd;clip-rule:evenodd;fill:#A09F9F;} .st300{fill-rule:evenodd;clip-rule:evenodd;fill:#545353;} .st301{fill-rule:evenodd;clip-rule:evenodd;fill:#B21F24;} .st302{fill-rule:evenodd;clip-rule:evenodd;fill:#96B4A7;} .st303{fill-rule:evenodd;clip-rule:evenodd;fill:#F2F9F7;} .st304{fill-rule:evenodd;clip-rule:evenodd;fill:#D8AA4F;} .st305{fill-rule:evenodd;clip-rule:evenodd;fill:#383938;} .st306{fill-rule:evenodd;clip-rule:evenodd;fill:#242424;} .st307{fill-rule:evenodd;clip-rule:evenodd;fill:#EBEBEB;} .st308{fill-rule:evenodd;clip-rule:evenodd;fill:#D7A729;} .st309{fill-rule:evenodd;clip-rule:evenodd;fill:#363736;} .st310{fill-rule:evenodd;clip-rule:evenodd;fill:#010101;} .st311{fill-rule:evenodd;clip-rule:evenodd;fill:#946828;} .st312{fill-rule:evenodd;clip-rule:evenodd;fill:#F3CD42;} .st313{fill-rule:evenodd;clip-rule:evenodd;fill:#4F4F4F;} .st314{fill-rule:evenodd;clip-rule:evenodd;fill:#CBCBCB;} .st315{fill-rule:evenodd;clip-rule:evenodd;fill:#2E3F44;} .st316{fill-rule:evenodd;clip-rule:evenodd;fill:#507481;} .st317{fill-rule:evenodd;clip-rule:evenodd;fill:#75A6AA;} .st318{fill-rule:evenodd;clip-rule:evenodd;fill:#88C4C8;} .st319{fill-rule:evenodd;clip-rule:evenodd;fill:#416162;} .st320{fill-rule:evenodd;clip-rule:evenodd;fill:#537D75;} .st321{fill-rule:evenodd;clip-rule:evenodd;fill:#1A1A1A;} .st322{fill-rule:evenodd;clip-rule:evenodd;fill:#B7B7B8;} .st323{fill-rule:evenodd;clip-rule:evenodd;fill:#4C4C4C;} .st324{fill-rule:evenodd;clip-rule:evenodd;fill:#686969;} .st325{font-size:20.3829px;} .st326{fill:#F48079;} .st327{fill:#435279;} .st328{fill:#43AFC1;} .st329{fill:#B6DFE7;} .st330{fill:#FDB723;} .st331{fill:#FED47B;} .st332{fill:#DFDFDE;} .st333{fill:#414141;} .st334{fill:#828282;} .st335{fill:#BD4B41;} .st336{fill:#ADADAD;} .st337{fill:#348491;} .st338{fill:#EF9721;} .st339{fill:#FAA626;} .st340{fill:#FFCE4F;} .st341{fill:#FFD373;} .st342{fill:#F6BF43;} .st343{fill:#DAF0F2;} .st344{fill:#854626;} .st345{fill:#AE643C;} .st346{fill:#E35E2F;} .st347{fill:#C44127;} .st348{fill:#93532F;} .st349{fill:#EADBB7;} .st350{fill:#BC795C;} .st351{fill:#0A324A;} .st352{fill:#2A5B90;} .st353{fill:#422C23;} .st354{fill:#87544E;} .st355{clip-path:url(#SVGID_13_);} .st356{fill:#716C60;} .st357{fill:#E2B488;} .st358{fill:#C0332F;} .st359{fill:#2F2D2C;} .st360{fill:#B8DFC8;} .st361{font-size:21.4904px;} .st362{clip-path:url(#SVGID_15_);} .st363{fill:#174991;} .st364{fill:#2D5972;} .st365{fill:#104C98;} .st366{fill:#1C3462;} .st367{fill:#D9D5D4;} .st368{fill:#CCC8C7;} .st369{fill:#B5B3B1;} .st370{fill:#C3BFBE;} .st371{fill:url(#SVGID_16_);} .st372{fill:#6F6148;} .st373{fill:url(#SVGID_17_);} .st374{clip-path:url(#SVGID_19_);} .st375{fill:#74858F;} .st376{fill:#D7F0FC;} .st377{fill:#8C8C8C;}
    </style>
    <path class="st0" d="M1920 3998.9L631.4 3239.6l-2.4-1.4c-4.7-2.9-9.4-6.2-12.8-8.3-18.9-12-16.7-22.4-11.1-29.3l798.8-472.9 53.1-31.3c-.2-.4.1-.5.7-.4l5.2-3c14.3-8.5 30.6-11.4 47.7-2.3l7.9 4.7c.7-.1 1.1 0 1 .3l364.9 214.9 32.7 19.3 3 1.8c.1-4.3 0-7.5 0-11.8v-90.2l-118.4-69.7-1257.2-740.9 871-513.5c-.1-.3.3-.4 1-.3l7.9-4.7c17.1-9.1 33.3-6.3 47.6 2.3l5.2 3c.6-.1.8 0 .7.4l53.1 31.3 389.1 230.1c-.2-36-.2-65.7-.4-101.7l-389.8-229.7c-.1-.1-.1-.2-.2-.3l-58.9-34.7c-1.7-1-3.4-1.9-5.1-2.7-13-6.3-27.4-7.6-42.5.5l-24.9 14.7c-1.4.8-2.7 1.8-3.9 2.8l-.4-.2-936 551.9-394.9-232.8c-.1-.1-.1-.2-.2-.3l-51.3-30.3c-1.7-1-5.9-3.6-7.6-4.5l-4-2.2v100.9c.8.5 3.7 1.9 5.3 2.8l5.2 3c.6-.1 0 0 .7.4l53.1 31.3 308.2 181.8L0 2238.1c-.2 35 0 68.4 0 102l458.8-270.5 895.4 528.3 19.4 11.4 1.3.7c5.5 3.4 25.7 18.4-4.3 36.6l-2.3 1.4c-.6.3-1.1.7-1.7 1L0 3453.4l-.3 3.6.3 4.7c0 36.2-.3 62.3 0 97.1l470.5-277.4c-.1-.3.3-.4 1-.3l7.9-4.7c17.1-9.1 33.3-6.3 47.6 2.3l5.2 3c.6-.1.8 0 .7.4l53.1 31.3 1334 787.1c-1.5-34.7.6-66.9 0-101.6zm-.2-3733.3c.7-18.9.2-33.7.2-58.2L1658.3 53.2c-.1-.1-.1-.2-.2-.3l-58.9-34.7c-1.7-1-3.4-1.9-5.1-2.7-13-6.3-27.4-7.6-42.5.5l-24.9 14.7c-1.4.8-2.7 1.8-3.9 2.8l-.4-.2L1 930.3v102l1543-909.8c-.1-.3.3-.4 1-.3l7.9-4.7c17.1-9.1 33.3-6.3 47.6 2.3l5.2 3c.6-.1.8 0 .7.4l53.1 31.3 260.6 153.8c0-13-.8-27.2-.3-42.7z"/>
    <g id="cross-sign-1">
      <path class="st1" d="M460.5 1943.5l-21.6-12.3 9.7-6v-2.1l-2.8-.1-1 .7-9 5.3-2.2-1.1-3.5 1.9 2.2 1.1-4.8 2.8 3.7 2.2 4.5-2.8 23.2 13.3z"/>
      <path class="st2" d="M461.7 1901.3l-.1 44c0 .3-.2.6-.5.8-.7.4-1.9.4-2.7 0-.4-.2-.6-.5-.6-.8l.1-44c0 .3.2.6.6.8.7.4 1.9.4 2.7 0 .3-.2.5-.5.5-.8z"/>
      <path class="st3" d="M461.1 1900.5c.7.4.7 1.1 0 1.5-.7.4-1.9.4-2.7 0-.7-.4-.7-1.1 0-1.5.8-.4 2-.4 2.7 0z"/>
      <path class="st4" d="M474.1 1908.9l-.9-.5-3.5-1.2.9.5z"/>
      <path class="st5" d="M453.3 1917.7l-.9-.5v6.4l.9.5z"/>
      <path class="st5" d="M470.6 1907.7l-.9-.5-17.3 10 .9.5z"/>
      <path class="st6" d="M453.3 1917.7v6.4l17.3-10 3.5-5.2-3.5-1.2z"/>
      <path class="st7" d="M449 1901.1l.8-.5 17.3 10-.8.5z"/>
      <path class="st7" d="M466.3 1911.1l.8-.5 3.5 5.2-.9.5z"/>
      <path class="st8" d="M466.3 1911.1l3.4 5.2-3.4 1.2-17.3-10v-6.4z"/>
    </g>
    <g id="cross-sign-2">
      <path class="st1" d="M702.1 3221.4l-21.7-12.4 9.7-6v-2l-2.7-.2-1.1.8-9 5.3-2.1-1.1-3.6 1.9 2.2 1.1-4.8 2.8 3.7 2.2 4.5-2.8 23.2 13.2z"/>
      <path class="st2" d="M703.2 3179.2l-.1 44c0 .3-.2.6-.5.8-.7.4-1.9.4-2.7 0-.4-.2-.6-.5-.6-.8l.1-44c0 .3.2.6.6.8.7.4 1.9.4 2.7 0 .3-.3.5-.6.5-.8z"/>
      <path class="st3" d="M702.6 3178.4c.7.4.7 1.1 0 1.5-.7.4-1.9.4-2.7 0-.7-.4-.7-1.1 0-1.5.8-.4 2-.4 2.7 0z"/>
      <path class="st4" d="M715.6 3186.8l-.9-.5-3.5-1.2.9.5z"/>
      <path class="st5" d="M694.8 3195.6l-.9-.5v6.3l.9.5zm17.3-10l-.9-.5-17.3 10 .9.5z"/>
      <path class="st6" d="M694.8 3195.6v6.3l17.3-10 3.5-5.1-3.5-1.2z"/>
      <path class="st7" d="M690.5 3179l.8-.5 17.4 10-.9.5z"/>
      <path class="st7" d="M707.8 3189l.9-.5 3.4 5.2-.8.5z"/>
      <path class="st8" d="M707.8 3189l3.5 5.2-3.5 1.1-17.3-10v-6.3z"/>
    </g>
    <g id="house-3">
      <path class="st9" d="M250.5 947.8l36.8 21.6-37.5 21.6-37.3-21.6z"/>
      <path class="st10" d="M310.9 940.9c-12.6-7.4-25.3-14.7-37.9-22.1-.1-.1-.3-.1-.5-.1l37.9 22.1c.2-.1.3 0 .5.1z"/>
      <path class="st2" d="M305.7 941.3v10.2l-15.2 1.3-23 23.3-38.1-17.7v-9.7z"/>
      <path class="st11" d="M267.5 1001.8l38.3-22.1-.1-31.9-19.2.7-19 20.7v32.6z"/>
      <path class="st6" d="M287.7 980l14.3-8.3v-16.5l-14.4 8.3z"/>
      <path class="st8" d="M271.2 999.5l12-6.9-.1-26.5-12 7z"/>
      <path class="st11" d="M287.1 963.2l15.3-8.8V972l-15.3 8.8v-17.6zm14.4-7.1l-13.3 7.7v15.3l13.3-7.7v-15.3zm-17.8 36.3l-.1-27.2-13 7.5.1 27.2 13-7.5zm-1-.1l-11 6.4-.1-25.3 11-6.4.1 25.3z"/>
      <path class="st12" d="M261.6 972.7c.3.2.7.3 1 .3.4 0 .9-.1 1.3-.4.4-.2.7-.5 1-.9l2.6-2.5v32.5l-37.9-22-.1-25.7 32.1 18.7z"/>
      <path class="st13" d="M244.5 924.4h20.4v29.1h-20.4z"/>
      <path class="st14 st6" d="M246.5 932.4l.1 14.4 8 4.7-.5-13.7zm8.4 5.4l-.3 13.7 8-8.5-.1-10.6zm-8.4-5.4l8 4.6 8-4.6-8-4.6-8 4.6zm4.2 0l3.9-2.2 3.8 2.2-3.9 2.2-3.8-2.2z"/>
      <path class="st15" d="M246.7 932.6l-.1 13.5 8 4.6 8-8.5-.3-9.6-7.8-4.3z"/>
      <path class="st6" d="M310.4 940.7l-37.9-22.1-23.2.5c-.1 0-.2.1-.3.1l37.5 26.3 22.5-.4c.2 0 .5-.1.7-.2.6-.4 1.2-1.1 1.5-2 .4-1.2 0-2.2-.8-2.2z"/>
      <path class="st5" d="M248.5 919.4c-.3.1-.5.4-.7.6l-23.1 26.3c-.8 1-1.2 2.3-.8 3 .1.2.2.3.3.3 12.6 7.4 25.3 14.7 37.9 22.1.3.2.8.2 1.2-.1.2-.1.5-.3.7-.6l22.4-25.5-37.4-26.3c-.2.1-.3.1-.5.2zm14.1 22.8l-8 8.5-8-4.6.1-13.4 7.7-4.4 7.8 4.4.4 9.5z"/>
    </g>
    <g id="house-2">
      <path class="st9" d="M341 897.5l36.8 21.6-37.5 21.6-37.2-21.7z"/>
      <path class="st10" d="M401.4 890.5c-12.6-7.4-25.3-14.7-37.9-22.1-.1-.1-.3-.1-.5-.1l37.9 22.1c.2 0 .4.1.5.1z"/>
      <path class="st2" d="M396.3 891v10.2l-15.3 1.3-23 23.3-38-17.7v-9.7z"/>
      <path class="st11" d="M358 951.5l38.3-22.1-.1-31.9-19.2.7-19 20.7v32.6z"/>
      <path class="st6" d="M378.2 929.7l14.4-8.3-.1-16.5-14.3 8.3z"/>
      <path class="st8" d="M361.7 949.2l12-6.9-.1-26.5-12 7z"/>
      <path class="st11" d="M377.7 912.9l15.3-8.8v17.6l-15.3 8.8v-17.6zm14.3-7.1l-13.3 7.7v15.3l13.3-7.7v-15.3zm-17.8 36.3l-.1-27.2-13 7.5.1 27.2 13-7.5zm-1-.1l-11 6.4-.1-25.3 11-6.4.1 25.3z"/>
      <path class="st12" d="M352.1 922.4c.3.2.7.3 1 .3.4 0 .9-.1 1.3-.4.4-.2.7-.5 1-.9l2.6-2.5v32.5l-37.9-22-.1-25.7 32.1 18.7z"/>
      <path class="st13" d="M335 874.1h20.4v29.1H335z"/>
      <g class="st14">
        <path class="st6" d="M337 882.1l.1 14.4 8 4.7-.5-13.7z"/>
        <path class="st6" d="M345.4 887.5l-.3 13.7 8-8.5-.1-10.6z"/>
        <path class="st6" d="M337 882.1l8 4.6 8-4.6-8-4.6-8 4.6zm4.2 0l3.9-2.2 3.8 2.2-3.9 2.2-3.8-2.2z"/>
      </g>
      <path class="st15" d="M337.3 882.3l-.2 13.5 8 4.6 8-8.5-.3-9.6-7.8-4.3z"/>
      <path class="st6" d="M401 890.4l-38-22-23.2.5c-.1 0-.2.1-.3.1l37.5 26.3 22.5-.4c.2 0 .5-.1.7-.2.6-.4 1.2-1.1 1.5-2 .4-1.3.1-2.3-.7-2.3z"/>
      <path class="st5" d="M339.1 869.1c-.3.1-.5.4-.7.6L315.2 896c-.8 1-1.2 2.3-.8 3 .1.2.2.3.3.3 12.6 7.4 25.3 14.7 37.9 22.1.3.2.8.2 1.2-.1.2-.1.5-.3.7-.6l22.4-25.5-37.5-26.3c0 .1-.2.1-.3.2zm14 22.8l-8 8.5-8-4.6.1-13.4 7.7-4.4 7.8 4.4.4 9.5z"/>
    </g>
    <g id="house-1">
      <path class="st9" d="M430.1 846.7l36.8 21.5-37.5 21.7-37.3-21.7z"/>
      <path class="st10" d="M490.5 839.7c-12.6-7.4-25.3-14.7-37.9-22.1-.1-.1-.3-.1-.5-.1l37.9 22.1c.2 0 .4 0 .5.1z"/>
      <path class="st2" d="M485.4 840.2v10.1l-15.3 1.3-23 23.3-38-17.6v-9.8z"/>
      <path class="st11" d="M447.1 900.6l38.3-22.1-.1-31.9-19.2.7-19 20.7v32.6z"/>
      <path class="st6" d="M467.3 878.8l14.3-8.3v-16.4l-14.3 8.3z"/>
      <path class="st8" d="M450.8 898.4l12-6.9-.1-26.5-12 6.9z"/>
      <path class="st11" d="M466.8 862.1l15.3-8.8v17.6l-15.3 8.8v-17.6zm14.3-7.1l-13.3 7.7V878l13.3-7.7V855zm-17.8 36.3l-.1-27.2-13 7.5.1 27.2 13-7.5zm-1-.1l-11 6.4-.1-25.3 11-6.4.1 25.3z"/>
      <path class="st12" d="M441.2 871.6c.3.2.7.3 1 .3.4 0 .9-.1 1.3-.4.4-.2.7-.5 1-.9l2.6-2.5v32.5l-37.9-22-.1-25.7 32.1 18.7z"/>
      <path class="st13" d="M424.1 823.3h20.4v29.1h-20.4z"/>
      <g class="st14">
        <path class="st6" d="M426.1 831.3l.1 14.4 8 4.6-.5-13.6z"/>
        <path class="st6" d="M434.5 836.7l-.3 13.6 8-8.5-.1-10.5zm-8.4-5.4l8 4.6 8-4.6-8-4.6-8 4.6zm4.2 0l3.9-2.2 3.8 2.2-3.9 2.2-3.8-2.2z"/>
      </g>
      <path class="st15" d="M426.3 831.5l-.1 13.4 8 4.6 8-8.4-.3-9.6-7.8-4.4z"/>
      <path class="st6" d="M490 839.6l-37.9-22.1-23.2.5c-.1 0-.2.1-.3.1l37.5 26.3 22.5-.4c.2 0 .5-.1.7-.2.6-.4 1.2-1.1 1.5-2 .4-1.3.1-2.2-.8-2.2z"/>
      <path class="st5" d="M428.1 818.2c-.3.1-.5.4-.7.6l-23.1 26.3c-.8 1-1.2 2.3-.8 3 .1.2.2.3.3.3 12.6 7.4 25.3 14.7 37.9 22.1.3.2.8.2 1.2-.1.2-.1.5-.3.7-.6l22.4-25.5-37.5-26.3c-.1.1-.2.1-.4.2zm14.1 22.9l-8 8.5-8-4.6.1-13.4 7.7-4.4 7.8 4.4.4 9.5z"/>
    </g>
    <g id="tree-9">
      <path class="st16" d="M309.1 1044.7l-7.6-4.3 7.1-3.9-19-2.3 3.9-2-14.7-2.3 3-1.7-13.8-2.6 5.5 7.4 2.6-1.4 5.6 7.7 2.2-1.9 6 9 8.3-4.5 7.9 4.4c.2.1.5.1.8.1h.4c.9-.2 1.7-.7 1.9-1.2.2-.2.2-.4-.1-.5z"/>
      <path class="st17" d="M308.7 1044.6c1 .6 1 1.5 0 2.1-.9.5-2.4.6-3.4.1-.1 0-.2-.1-.2-.1-.1 0-.1-.1-.2-.1-.8-.6-.7-1.4.2-2 .9-.5 2.6-.5 3.6 0z"/>
      <path class="st17" d="M304.3 1016.1h5.2v29.6h-5.2z"/>
      <path class="st18" d="M306.9 1007.1s-13.6 25.5-13.6 27c0 2 1.3 4 4 5.6 5.3 3.1 13.9 3.1 19.2 0 2.7-1.5 4-3.6 3.9-5.6 0-1.5-13.5-27-13.5-27z"/>
      <path class="st19" d="M316.5 1039.7c2.7-1.5 4-3.6 3.9-5.6 0-1.4-13.6-27-13.6-27v34.8c3.5.1 7-.7 9.7-2.2z"/>
      <path class="st16" d="M317.7 1028.1c-4-8-10.9-21-10.9-21s-6.9 13-10.9 20.9c.5 1.1 1.5 2.1 3 3 4.4 2.5 11.5 2.6 15.9 0 1.5-.8 2.5-1.8 2.9-2.9z"/>
      <path class="st18" d="M306.9 1002s-11.3 21.1-11.3 22.4c0 1.7 1.1 3.3 3.3 4.6 4.4 2.5 11.5 2.6 15.9 0 2.2-1.3 3.3-2.9 3.3-4.6 0-1.3-11.2-22.4-11.2-22.4z"/>
      <path class="st19" d="M314.9 1029c2.2-1.3 3.3-2.9 3.3-4.6 0-1.2-11.3-22.3-11.3-22.3v28.9c2.9-.1 5.8-.7 8-2z"/>
      <path class="st16" d="M306.9 1002s-3.5 6.7-6.7 12.7c.4.4.8.9 1.5 1.2 2.9 1.7 7.5 1.7 10.4 0 .6-.4 1.1-.8 1.4-1.2-3.1-6-6.6-12.7-6.6-12.7z"/>
      <path class="st18" d="M306.9 996.2s-7.4 13.8-7.4 14.6c0 1.1.7 2.2 2.2 3 2.9 1.7 7.5 1.7 10.4 0 1.4-.8 2.1-1.9 2.1-3 0-.8-7.3-14.6-7.3-14.6z"/>
      <path class="st19" d="M312.1 1013.8c1.4-.8 2.1-1.9 2.1-3 0-.8-7.4-14.6-7.4-14.6v18.9c1.9 0 3.8-.4 5.3-1.3z"/>
    </g>
    <g id="tree-8">
      <path class="st16" d="M290.1 2034.7l-7.6-4.3 7.1-3.9-19-2.3 3.9-2-14.7-2.3 3-1.7-13.8-2.6 5.5 7.4 2.6-1.4 5.6 7.7 2.2-1.9 6 9 8.3-4.5 7.9 4.4c.2.1.5.1.8.1h.4c.9-.2 1.7-.7 1.9-1.2.2-.2.2-.4-.1-.5z"/>
      <path class="st17" d="M289.7 2034.7c1 .6 1 1.5 0 2.1-.9.5-2.4.6-3.4.1-.1 0-.2-.1-.2-.1-.1 0-.1-.1-.2-.1-.8-.6-.7-1.4.2-2 .9-.6 2.6-.6 3.6 0z"/>
      <path class="st17" d="M285.3 2006.2h5.2v29.6h-5.2z"/>
      <path class="st18" d="M287.9 1997.1s-13.6 25.5-13.6 27c0 2 1.3 4 4 5.6 5.3 3.1 13.9 3.1 19.2 0 2.7-1.5 4-3.6 3.9-5.6 0-1.4-13.5-27-13.5-27z"/>
      <path class="st19" d="M297.5 2029.7c2.7-1.5 4-3.6 3.9-5.6 0-1.4-13.6-27-13.6-27v34.8c3.6.1 7.1-.7 9.7-2.2z"/>
      <path class="st16" d="M298.8 2018.1c-4-8-10.9-21-10.9-21s-6.9 13-10.9 20.9c.5 1.1 1.5 2.1 3 3 4.4 2.5 11.5 2.6 15.9 0 1.4-.8 2.4-1.8 2.9-2.9z"/>
      <path class="st18" d="M287.9 1992s-11.3 21.1-11.3 22.4c0 1.7 1.1 3.3 3.3 4.6 4.4 2.5 11.5 2.6 15.9 0 2.2-1.3 3.3-2.9 3.3-4.6 0-1.2-11.2-22.4-11.2-22.4z"/>
      <path class="st19" d="M295.9 2019c2.2-1.3 3.3-2.9 3.3-4.6 0-1.2-11.3-22.3-11.3-22.3v28.9c2.9-.1 5.8-.7 8-2z"/>
      <path class="st16" d="M287.9 1992s-3.5 6.7-6.7 12.7c.4.4.8.9 1.5 1.2 2.9 1.7 7.5 1.7 10.4 0 .6-.4 1.1-.8 1.4-1.2-3.1-6-6.6-12.7-6.6-12.7z"/>
      <path class="st18" d="M287.9 1986.2s-7.4 13.8-7.4 14.6c0 1.1.7 2.2 2.2 3 2.9 1.7 7.5 1.7 10.4 0 1.4-.8 2.1-1.9 2.1-3 0-.8-7.3-14.6-7.3-14.6z"/>
      <path class="st19" d="M293.1 2003.8c1.4-.8 2.1-1.9 2.1-3 0-.8-7.4-14.6-7.4-14.6v18.9c2 0 3.8-.4 5.3-1.3z"/>
    </g>
    <g id="tree-7">
      <path class="st16" d="M218.8 2079.9l-7.6-4.3 7.1-3.9-19-2.3 3.9-2-14.7-2.3 3-1.7-13.8-2.6 5.5 7.4 2.6-1.4 5.6 7.7 2.2-1.9 6 9 8.3-4.5 7.9 4.4c.2.1.5.1.8.1h.4c.9-.2 1.7-.7 1.9-1.2.2-.2.1-.4-.1-.5z"/>
      <path class="st17" d="M218.4 2079.9c1 .6 1 1.5 0 2.1-.9.5-2.4.6-3.4.1-.1 0-.2-.1-.2-.1-.1 0-.1-.1-.2-.1-.8-.6-.7-1.4.2-2 .9-.6 2.6-.6 3.6 0z"/>
      <path class="st17" d="M213.9 2051.4h5.2v29.6h-5.2z"/>
      <path class="st18" d="M216.5 2042.4s-13.6 25.5-13.6 27c0 2 1.3 4 4 5.6 5.3 3.1 13.9 3.1 19.2 0 2.7-1.5 4-3.6 3.9-5.6.1-1.5-13.5-27-13.5-27z"/>
      <path class="st19" d="M226.2 2074.9c2.7-1.5 4-3.6 3.9-5.6 0-1.4-13.6-27-13.6-27v34.8c3.5.1 7-.6 9.7-2.2z"/>
      <path class="st16" d="M227.4 2063.4c-4-8-10.9-21-10.9-21s-6.9 13-10.9 20.9c.5 1.1 1.5 2.1 3 3 4.4 2.5 11.5 2.6 15.9 0 1.5-.8 2.4-1.8 2.9-2.9z"/>
      <path class="st18" d="M216.5 2037.3s-11.3 21.1-11.3 22.4c0 1.7 1.1 3.3 3.3 4.6 4.4 2.5 11.5 2.6 15.9 0 2.2-1.3 3.3-2.9 3.3-4.6.1-1.3-11.2-22.4-11.2-22.4z"/>
      <path class="st19" d="M224.5 2064.2c2.2-1.3 3.3-2.9 3.3-4.6 0-1.2-11.3-22.3-11.3-22.3v28.9c2.9-.1 5.8-.7 8-2z"/>
      <path class="st16" d="M216.5 2037.3s-3.5 6.7-6.7 12.7c.4.4.8.9 1.5 1.2 2.9 1.7 7.5 1.7 10.4 0 .6-.4 1.1-.8 1.4-1.2-3-6.1-6.6-12.7-6.6-12.7z"/>
      <path class="st18" d="M216.5 2031.5s-7.4 13.8-7.4 14.6c0 1.1.7 2.2 2.2 3 2.9 1.7 7.5 1.7 10.4 0 1.4-.8 2.1-1.9 2.1-3 .1-.8-7.3-14.6-7.3-14.6z"/>
      <path class="st19" d="M221.8 2049.1c1.4-.8 2.1-1.9 2.1-3 0-.8-7.4-14.6-7.4-14.6v18.9c1.9-.1 3.8-.5 5.3-1.3z"/>
    </g>
    <g id="tree-6">
      <path class="st16" d="M1353.6 1403.1l-10.4-5.8 9.8-5.3-26-3.2 5.4-2.7-20.1-3.2 4.1-2.3-18.9-3.6 7.6 10.1 3.5-1.9 7.7 10.6 3-2.6 8.2 12.4 11.4-6.2 10.8 6c.3.1.6.2 1.2.2h.6c1.2-.3 2.3-.9 2.6-1.6-.1-.5-.2-.8-.5-.9z"/>
      <path class="st17" d="M1353 1403c1.4.8 1.4 2.1 0 2.9-1.3.7-3.3.8-4.7.2-.1-.1-.2-.1-.3-.2-.1-.1-.2-.1-.3-.2-1.1-.8-1-2 .3-2.7 1.4-.8 3.6-.8 5 0z"/>
      <path class="st17" d="M1347 1364h7.1v40.5h-7.1z"/>
      <path class="st18" d="M1350.5 1351.6s-18.6 34.9-18.6 37c0 2.8 1.9 5.5 5.5 7.6 7.3 4.2 19.1 4.2 26.3 0 3.6-2.1 5.4-4.9 5.4-7.7 0-1.9-18.6-36.9-18.6-36.9z"/>
      <path class="st19" d="M1363.7 1396.2c3.6-2.1 5.4-4.9 5.4-7.7 0-2-18.6-37-18.6-37v47.8c4.8.1 9.6-1 13.2-3.1z"/>
      <path class="st16" d="M1365.4 1380.4c-5.4-10.9-14.9-28.8-14.9-28.8s-9.5 17.8-14.9 28.7c.7 1.5 2 2.9 4 4.1 6 3.5 15.8 3.5 21.8 0 2.1-1.1 3.4-2.5 4-4z"/>
      <path class="st18" d="M1350.5 1344.6s-15.4 29-15.4 30.6c0 2.3 1.5 4.6 4.6 6.3 6 3.5 15.8 3.5 21.8 0 3-1.7 4.5-4 4.5-6.3-.1-1.6-15.5-30.6-15.5-30.6z"/>
      <path class="st19" d="M1361.5 1381.6c3-1.7 4.5-4 4.5-6.3 0-1.6-15.4-30.6-15.4-30.6v39.6c3.9-.1 7.9-1 10.9-2.7z"/>
      <path class="st16" d="M1350.5 1344.6s-4.9 9.1-9.1 17.4c.5.6 1.2 1.2 2 1.7 3.9 2.3 10.3 2.3 14.3 0 .8-.5 1.5-1.1 2-1.6-4.3-8.4-9.2-17.5-9.2-17.5z"/>
      <path class="st18" d="M1350.5 1336.7s-10.1 18.9-10.1 20c0 1.5 1 3 3 4.1 3.9 2.3 10.3 2.3 14.3 0 2-1.1 2.9-2.6 2.9-4.1 0-1.1-10.1-20-10.1-20z"/>
      <path class="st19" d="M1357.7 1360.8c2-1.1 2.9-2.6 2.9-4.1 0-1.1-10.1-20-10.1-20v25.9c2.6-.1 5.2-.6 7.2-1.8z"/>
    </g>
    <g id="tree-5">
      <path class="st16" d="M1493.7 2784.8l-11.4-6.4 10.7-5.8-28.5-3.5 5.9-3-22-3.5 4.5-2.5-20.7-4 8.3 11.1 3.9-2.1 8.4 11.6 3.3-2.8 9 13.6 12.5-6.8 11.9 6.6c.3.1.7.2 1.3.2l.3-.1h.3c1.3-.3 2.5-1 2.9-1.7-.1-.4-.3-.7-.6-.9z"/>
      <path class="st17" d="M1493 2784.8c1.5.9 1.5 2.3 0 3.2-1.4.8-3.6.9-5.2.2-.1-.1-.2-.1-.4-.2-.1-.1-.2-.1-.3-.2-1.2-.9-1.1-2.2.3-3 1.6-.9 4.1-.9 5.6 0z"/>
      <path class="st17" d="M1486.4 2742.1h7.8v44.3h-7.8z"/>
      <path class="st18" d="M1490.3 2728.5s-20.4 38.2-20.4 40.5c0 3 2 6 6 8.4 8 4.6 20.9 4.6 28.8 0 4-2.3 5.9-5.3 5.9-8.4 0-2.2-20.3-40.5-20.3-40.5z"/>
      <path class="st19" d="M1504.8 2777.4c4-2.3 5.9-5.3 5.9-8.4 0-2.2-20.4-40.4-20.4-40.4v52.3c5.2-.1 10.5-1.2 14.5-3.5z"/>
      <path class="st16" d="M1506.6 2760c-5.9-11.9-16.3-31.5-16.3-31.5s-10.4 19.5-16.3 31.4c.7 1.6 2.2 3.2 4.4 4.5 6.6 3.8 17.3 3.8 23.9 0 2.2-1.2 3.6-2.7 4.3-4.4z"/>
      <path class="st18" d="M1490.3 2720.8s-16.9 31.7-16.9 33.5c0 2.5 1.7 5 5 6.9 6.6 3.8 17.3 3.8 23.9 0 3.3-1.9 4.9-4.4 4.9-6.9 0-1.7-16.9-33.5-16.9-33.5z"/>
      <path class="st19" d="M1502.3 2761.3c3.3-1.9 4.9-4.4 4.9-6.9 0-1.8-16.9-33.5-16.9-33.5v43.3c4.3 0 8.7-1 12-2.9z"/>
      <path class="st16" d="M1490.3 2720.8s-5.3 10-10 19.1c.5.7 1.3 1.3 2.2 1.8 4.3 2.5 11.3 2.5 15.6 0 .9-.5 1.6-1.2 2.2-1.8-4.7-9.1-10-19.1-10-19.1z"/>
      <path class="st18" d="M1490.3 2712.2s-11 20.7-11 21.9c0 1.6 1.1 3.3 3.3 4.5 4.3 2.5 11.3 2.5 15.6 0 2.2-1.2 3.2-2.9 3.2-4.5-.1-1.2-11.1-21.9-11.1-21.9z"/>
      <path class="st19" d="M1498.1 2738.6c2.2-1.2 3.2-2.9 3.2-4.5 0-1.2-11-21.9-11-21.9v28.3c2.8 0 5.7-.6 7.8-1.9z"/>
    </g>
    <g id="tree-4">
      <path class="st16" d="M1278.7 1452.1l-7.6-4.3 7.1-3.9-19-2.3 3.9-2-14.7-2.3 3-1.7-13.8-2.6 5.5 7.4 2.6-1.4 5.6 7.7 2.2-1.9 6 9 8.3-4.5 7.9 4.4c.2.1.5.1.8.1h.4c.9-.2 1.7-.7 1.9-1.2.2-.2.1-.4-.1-.5z"/>
      <path class="st17" d="M1278.3 1452c1 .6 1 1.5 0 2.1-.9.5-2.4.6-3.4.1-.1 0-.2-.1-.2-.1-.1 0-.1-.1-.2-.1-.8-.6-.7-1.4.2-2 .9-.5 2.5-.5 3.6 0z"/>
      <path class="st17" d="M1273.8 1423.5h5.2v29.6h-5.2z"/>
      <path class="st18" d="M1276.4 1414.5s-13.6 25.5-13.6 27c0 2 1.3 4 4 5.6 5.3 3.1 13.9 3.1 19.2 0 2.7-1.5 4-3.6 3.9-5.6.1-1.5-13.5-27-13.5-27z"/>
      <path class="st19" d="M1286.1 1447.1c2.7-1.5 4-3.6 3.9-5.6 0-1.4-13.6-27-13.6-27v34.8c3.5.1 7-.7 9.7-2.2z"/>
      <path class="st16" d="M1287.3 1435.5c-4-8-10.9-21-10.9-21s-6.9 13-10.9 20.9c.5 1.1 1.5 2.1 3 3 4.4 2.5 11.5 2.6 15.9 0 1.5-.8 2.4-1.8 2.9-2.9z"/>
      <path class="st18" d="M1276.4 1409.4s-11.3 21.1-11.3 22.4c0 1.7 1.1 3.3 3.3 4.6 4.4 2.5 11.5 2.6 15.9 0 2.2-1.3 3.3-2.9 3.3-4.6.1-1.3-11.2-22.4-11.2-22.4z"/>
      <path class="st19" d="M1284.4 1436.4c2.2-1.3 3.3-2.9 3.3-4.6 0-1.2-11.3-22.3-11.3-22.3v28.9c2.9-.1 5.8-.7 8-2z"/>
      <path class="st16" d="M1276.4 1409.4s-3.5 6.7-6.7 12.7c.4.4.8.9 1.5 1.2 2.9 1.7 7.5 1.7 10.4 0 .6-.4 1.1-.8 1.4-1.2-3-6-6.6-12.7-6.6-12.7z"/>
      <path class="st18" d="M1276.4 1403.6s-7.4 13.8-7.4 14.6c0 1.1.7 2.2 2.2 3 2.9 1.7 7.5 1.7 10.4 0 1.4-.8 2.1-1.9 2.1-3 .1-.8-7.3-14.6-7.3-14.6z"/>
      <path class="st19" d="M1281.6 1421.2c1.4-.8 2.1-1.9 2.1-3 0-.8-7.4-14.6-7.4-14.6v18.9c2 0 3.9-.4 5.3-1.3z"/>
    </g>
    <g id="tree-3">
      <path class="st16" d="M393.6 991.6l-7.6-4.3 7.1-3.9-19-2.3 3.9-2-14.7-2.3 3-1.7-13.8-2.6 5.5 7.4 2.6-1.4 5.6 7.7 2.2-1.9 6 9 8.3-4.5 7.9 4.4c.2.1.5.1.8.1h.4c.9-.2 1.7-.7 1.9-1.2.2-.1.1-.3-.1-.5z"/>
      <path class="st17" d="M393.1 991.6c1 .6 1 1.5 0 2.1-.9.5-2.4.6-3.4.1-.1 0-.2-.1-.2-.1-.1 0-.1-.1-.2-.1-.8-.6-.7-1.4.2-2 .9-.6 2.6-.6 3.6 0z"/>
      <path class="st17" d="M388.7 963.1h5.2v29.6h-5.2z"/>
      <path class="st18" d="M391.3 954.1s-13.6 25.5-13.6 27c0 2 1.3 4 4 5.6 5.3 3.1 13.9 3.1 19.2 0 2.7-1.5 4-3.6 3.9-5.6 0-1.5-13.5-27-13.5-27z"/>
      <path class="st19" d="M400.9 986.6c2.7-1.5 4-3.6 3.9-5.6 0-1.4-13.6-27-13.6-27v34.8c3.6.1 7.1-.6 9.7-2.2z"/>
      <path class="st16" d="M402.2 975.1c-4-8-10.9-21-10.9-21s-6.9 13-10.9 20.9c.5 1.1 1.5 2.1 3 3 4.4 2.5 11.5 2.6 15.9 0 1.4-.8 2.4-1.8 2.9-2.9z"/>
      <path class="st18" d="M391.3 949S380 970.1 380 971.4c0 1.7 1.1 3.3 3.3 4.6 4.4 2.5 11.5 2.6 15.9 0 2.2-1.3 3.3-2.9 3.3-4.6 0-1.3-11.2-22.4-11.2-22.4z"/>
      <path class="st19" d="M399.3 975.9c2.2-1.3 3.3-2.9 3.3-4.6 0-1.2-11.3-22.3-11.3-22.3v28.9c2.9 0 5.8-.7 8-2z"/>
      <path class="st16" d="M391.3 949s-3.5 6.7-6.7 12.7c.4.4.8.9 1.5 1.2 2.9 1.7 7.5 1.7 10.4 0 .6-.4 1.1-.8 1.4-1.2-3.1-6.1-6.6-12.7-6.6-12.7z"/>
      <path class="st18" d="M391.3 943.2s-7.4 13.8-7.4 14.6c0 1.1.7 2.2 2.2 3 2.9 1.7 7.5 1.7 10.4 0 1.4-.8 2.1-1.9 2.1-3 0-.8-7.3-14.6-7.3-14.6z"/>
      <path class="st19" d="M396.5 960.8c1.4-.8 2.1-1.9 2.1-3 0-.8-7.4-14.6-7.4-14.6v18.9c2 0 3.9-.5 5.3-1.3z"/>
    </g>
    <g id="tree-2">
      <path class="st16" d="M481.6 942.4l-7.6-4.3 7.1-3.9-19-2.3 3.9-2-14.7-2.3 3-1.7-13.8-2.6 5.5 7.4 2.6-1.4 5.6 7.7 2.2-1.9 6 9 8.3-4.5 7.9 4.4c.2.1.5.1.8.1h.4c.9-.2 1.7-.7 1.9-1.2.2-.2.2-.4-.1-.5z"/>
      <path class="st17" d="M481.2 942.4c1 .6 1 1.5 0 2.1-.9.5-2.4.6-3.4.1-.1 0-.2-.1-.2-.1-.1 0-.1-.1-.2-.1-.8-.6-.7-1.4.2-2 .9-.6 2.6-.6 3.6 0z"/>
      <path class="st17" d="M476.8 913.9h5.2v29.6h-5.2z"/>
      <path class="st18" d="M479.4 904.9s-13.6 25.5-13.6 27c0 2 1.3 4 4 5.6 5.3 3.1 13.9 3.1 19.2 0 2.7-1.5 4-3.6 3.9-5.6 0-1.5-13.5-27-13.5-27z"/>
      <path class="st19" d="M489 937.4c2.7-1.5 4-3.6 3.9-5.6 0-1.4-13.6-27-13.6-27v34.8c3.6.1 7.1-.7 9.7-2.2z"/>
      <path class="st16" d="M490.3 925.8c-4-8-10.9-21-10.9-21s-6.9 13-10.9 20.9c.5 1.1 1.5 2.1 3 3 4.4 2.5 11.5 2.6 15.9 0 1.4-.8 2.4-1.8 2.9-2.9z"/>
      <path class="st18" d="M479.4 899.7s-11.3 21.1-11.3 22.4c0 1.7 1.1 3.3 3.3 4.6 4.4 2.5 11.5 2.6 15.9 0 2.2-1.3 3.3-2.9 3.3-4.6 0-1.2-11.2-22.4-11.2-22.4z"/>
      <path class="st19" d="M487.4 926.7c2.2-1.3 3.3-2.9 3.3-4.6 0-1.2-11.3-22.3-11.3-22.3v28.9c2.9-.1 5.8-.7 8-2z"/>
      <path class="st16" d="M479.4 899.7s-3.5 6.7-6.7 12.7c.4.4.8.9 1.5 1.2 2.9 1.7 7.5 1.7 10.4 0 .6-.4 1.1-.8 1.4-1.2-3.1-6-6.6-12.7-6.6-12.7z"/>
      <path class="st18" d="M479.4 893.9s-7.4 13.8-7.4 14.6c0 1.1.7 2.2 2.2 3 2.9 1.7 7.5 1.7 10.4 0 1.4-.8 2.1-1.9 2.1-3 0-.7-7.3-14.6-7.3-14.6z"/>
      <path class="st19" d="M484.6 911.6c1.4-.8 2.1-1.9 2.1-3 0-.8-7.4-14.6-7.4-14.6v18.9c2-.1 3.8-.5 5.3-1.3z"/>
    </g>
    <g id="tree-1">
      <path class="st16" d="M1581.8 205.7l-10.9-6.1 10.2-5.5-27.1-3.3 5.6-2.8-21-3.3 4.3-2.4-19.7-3.8 7.9 10.6 3.7-2 8 11 3.1-2.7 8.5 12.9 11.9-6.5 11.3 6.3c.3.1.7.2 1.2.2l.3-.1h.3c1.2-.3 2.4-1 2.7-1.7.1-.3 0-.6-.3-.8z"/>
      <path class="st17" d="M1581.2 205.7c1.5.8 1.5 2.2 0 3-1.3.8-3.4.8-4.9.2-.1-.1-.2-.1-.3-.2-.1-.1-.2-.1-.3-.2-1.1-.8-1.1-2.1.3-2.8 1.4-.8 3.7-.8 5.2 0z"/>
      <path class="st17" d="M1574.8 165h7.4v42.2h-7.4z"/>
      <path class="st18" d="M1578.5 152.1s-19.4 36.4-19.4 38.5c0 2.9 1.9 5.8 5.7 8 7.6 4.4 19.9 4.4 27.4 0 3.8-2.2 5.7-5.1 5.6-8 .1-2-19.3-38.5-19.3-38.5z"/>
      <path class="st19" d="M1592.3 198.6c3.8-2.2 5.7-5.1 5.6-8 0-2.1-19.4-38.5-19.4-38.5v49.8c5 0 10-1.1 13.8-3.3z"/>
      <path class="st16" d="M1594.1 182.1c-5.7-11.4-15.6-30-15.6-30s-9.9 18.5-15.5 29.9c.7 1.6 2.1 3 4.2 4.3 6.3 3.6 16.5 3.6 22.8 0 2-1.2 3.4-2.6 4.1-4.2z"/>
      <path class="st18" d="M1578.6 144.8s-16.1 30.2-16.1 31.9c0 2.4 1.6 4.8 4.7 6.6 6.3 3.6 16.5 3.6 22.8 0 3.1-1.8 4.7-4.2 4.7-6.6-.1-1.7-16.1-31.9-16.1-31.9z"/>
      <path class="st19" d="M1590 183.3c3.1-1.8 4.7-4.2 4.7-6.6 0-1.7-16.1-31.9-16.1-31.9V186c4.1.1 8.2-.8 11.4-2.7z"/>
      <path class="st16" d="M1578.6 144.8s-5.1 9.5-9.5 18.1c.5.6 1.2 1.2 2.1 1.7 4.1 2.4 10.8 2.4 14.9 0 .9-.5 1.6-1.1 2.1-1.7-4.6-8.6-9.6-18.1-9.6-18.1z"/>
      <path class="st18" d="M1578.5 136.5s-10.5 19.7-10.5 20.9c0 1.6 1 3.1 3.1 4.3 4.1 2.4 10.8 2.4 14.9 0 2-1.2 3.1-2.8 3-4.3 0-1.1-10.5-20.9-10.5-20.9z"/>
      <path class="st19" d="M1586 161.7c2-1.2 3.1-2.8 3-4.3 0-1.1-10.5-20.8-10.5-20.8v26.9c2.7 0 5.4-.6 7.5-1.8z"/>
    </g>
    <g id="store-building">
      <path class="st16" d="M1539.1 3640.5l99.4 57.4-71.7 42.3-99.8-57.8z"/>
      <path class="st20" d="M1467.4 3615.9l99.4 57.5v66.8l-99.8-57.8z"/>
      <path class="st21" d="M1606.7 3650.4l-39.9 23v66.8l39.6-22.8z"/>
      <path class="st22" d="M1592.2 3707.5l6.7-3.8v3.4l-6.7 3.8zm0 8.1l6.7-3.9v3.4l-6.7 3.9zm-3.4-2l6.7-3.9v3.4l-6.7 3.9zm7.4-4.3l6.7-3.9v3.4l-6.7 3.9zm-21.4-27.9l6.7-3.8v3.4l-6.7 3.8zm-2 24l6.7-3.8-.1 3.4-6.7 3.8zm23.4-26l6.7-3.8v3.4l-6.7 3.8zm-24.8 0l6.7-3.8v3.4l-6.7 3.8zm7.4-4.3l6.7-3.8v3.4l-6.7 3.8z"/>
      <path class="st23" d="M1467.3 3615.7l99.4 57.6v37c0 3.5-2.7 4.9-5.7 3.2-3.1-1.8-5.5-6-5.5-9.6 0 3.5-2.5 4.9-5.5 3.2-3-1.8-5.5-6-5.5-9.6 0 3.5-2.5 4.9-5.5 3.2-3.1-1.8-5.5-6-5.5-9.6 0 3.5-2.5 4.9-5.5 3.2-3-1.8-5.5-6-5.5-9.6 0 3.5-2.5 4.9-5.5 3.2-3.1-1.8-5.6-6.1-5.6-9.6 0 3.5-2.6 4.9-5.6 3.1-3-1.8-5.5-6-5.5-9.6 0 3.5-2.5 4.9-5.5 3.2-3-1.8-5.5-6-5.5-9.6 0 3.5-2.5 4.9-5.5 3.2-3-1.8-5.5-6-5.5-9.6 0 3.5-2.5 4.9-5.5 3.2-3-1.8-5.5-6-5.5-9.6v-36.9z"/>
      <path class="st24" d="M1506.2 3705.1v-42.9h20.9v55z"/>
      <path class="st25" d="M1527.1 3693.3v23.9l-20.9-12.1v-.1z"/>
      <path class="st26" d="M1503.6 3661l-32.3-29.9v16.6l-.1 19.9 32.4 18.7V3661z"/>
      <g class="st14">
        <path class="st27" d="M1494.1 3646.2c-.8-.1-1.6-.3-2.6-.9-.5-.3-.9-.6-1.3-1l13.4 28.6v-5.5l-9.5-21.2z"/>
        <path class="st28" d="M1471.3 3631.1v10.7l12.5 33-2.9-1.7-9.6-25.5-.1 19.9 32.3 18.7.1-34c-1.7-1.2-3.2-2.9-4.2-4.9l-3.1-1.8c-.6.5-1.4.7-2.3.6l9.5 21.4v5.5l-13.4-28.6c-1.4-1.1-2.6-2.7-3.5-4.4l-3.1-1.8 19.9 42.8v5.3l-9.8-5.7-20.4-48.4-1.9-1.1z"/>
        <path class="st27" d="M1473.3 3632.2l20.4 48.4 9.8 5.7v-5.3l-20-42.7c-1.2.8-2.9.8-4.7-.3-1.9-1.1-3.6-3.1-4.8-5.3l-.7-.5z"/>
        <path class="st23" d="M1471.3 3631.1v10.7l12.5 33-2.9-1.7-9.6-25.5-.1 19.9 32.3 18.7.1-34c-1.7-1.2-3.2-2.9-4.2-4.9l-3.1-1.8c-.6.5-1.4.7-2.3.6l9.5 21.4v5.5l-13.4-28.6c-1.4-1.1-2.6-2.7-3.5-4.4l-3.1-1.8 19.9 42.8v5.3l-9.8-5.7-20.4-48.4-1.9-1.1z"/>
        <path class="st24" d="M1503.6 3661l-32.2-29.9v30.1c.5.4.9.8 1.4 1 3.1 1.8 5.5.4 5.5-3.2 0 3.5 2.4 7.8 5.5 9.6 3 1.8 5.5.3 5.5-3.2 0 3.5 2.4 7.8 5.5 9.6 3.1 1.8 5.5.4 5.5-3.2 0 2.6 1.4 5.7 3.3 7.8V3661z"/>
        <path class="st27" d="M1471.3 3641.8v5.9l9.6 25.5 2.9 1.6zm2-9.6l20.4 48.4 9.8 5.7v-5.3l-20-42.7c-1.2.8-2.9.8-4.7-.3-1.9-1.1-3.6-3.1-4.8-5.3l-.7-.5z"/>
        <path class="st29" d="M1485.2 3634.3c0 1.8-.6 3.2-1.5 3.9l3.1 1.8c-1-1.8-1.6-3.8-1.6-5.7zm12.7 7.4c0 1.8-.6 3.2-1.6 3.9l3.1 1.8c-.9-1.9-1.5-3.9-1.5-5.7zm25.7 14.9c0 1.8-.6 3.2-1.6 3.9l3.1 1.8c-.9-1.9-1.5-3.9-1.5-5.7zm12.7 7.3c0 1.8-.6 3.2-1.5 3.9l3.1 1.8c-1-1.8-1.6-3.8-1.6-5.7z"/>
        <path class="st23" d="M1549.1 3676.2l13.4 27-.1 17.3-5.5-3.2-22.3-49.4c-.6.5-1.4.7-2.3.6l21.2 46.9-4.1-2.4-19.3-43.7-.1 22.7 6.9 13.8-7-4 32.3 18.7.1-36.5-13.2-7.8z"/>
        <path class="st24" d="M1549.1 3676.2l-1.7-1c-1.2.9-2.9.9-4.8-.2l-10.2-6.5c-.7-.1-1.4-.3-2.1-.7v1.5l-.1 22.7v3c1.9.1 3.3-1.3 3.3-3.9 0 3.5 2.5 7.8 5.5 9.6 3 1.8 5.5.4 5.5-3.2 0 3.5 2.4 7.8 5.5 9.6 3 1.8 5.5.4 5.5-3.2 0 3.5 2.5 7.8 5.5 9.6.5.3 1 .5 1.5.6v-10.9l.1-19.2-13.5-7.8z"/>
        <path class="st27" d="M1530.2 3692v9.8l7 4zm2.2-23.5c-.7-.1-1.4-.3-2.1-.7v1.5l19.3 43.7 4.1 2.4-21.3-46.9zm2.3-.7l22.3 49.5 5.5 3.2.1-17.3-13.4-27-1.7-1c-1.2.9-2.9.9-4.8-.2s-3.6-3.1-4.8-5.3l-3.2-1.9z"/>
        <path class="st29" d="M1547.4 3675.2l1.7 1 1.4.8c-1-1.8-1.5-3.9-1.5-5.7 0 1.8-.6 3.1-1.6 3.9z"/>
      </g>
      <path class="st29" d="M1467.3 3615.7l11 6.4-17.5 18.5-11-6.4z"/>
      <path class="st30" d="M1449.8 3634.2c0 3.5 2.4 7.8 5.5 9.6 3.1 1.8 5.5.4 5.5-3.2l-11-6.4z"/>
      <path class="st11" d="M1471.8 3646.9l17.5-18.4-11-6.4-17.5 18.5z"/>
      <path class="st31" d="M1460.8 3640.6c0 3.5 2.5 7.8 5.5 9.6 3 1.8 5.5.3 5.5-3.2l-11-6.4z"/>
      <path class="st11" d="M1494 3659.8l17.5-18.5-11.1-6.5-17.6 18.5z"/>
      <path class="st29" d="M1482.8 3653.3l17.6-18.5-11.1-6.3-17.5 18.4z"/>
      <path class="st30" d="M1471.8 3646.9c0 3.5 2.4 7.8 5.5 9.6 3 1.8 5.5.4 5.5-3.2l-11-6.4z"/>
      <path class="st31" d="M1482.8 3653.3c0 3.5 2.5 7.8 5.5 9.6 3 1.8 5.6.4 5.6-3.1l-11.1-6.5z"/>
      <path class="st29" d="M1505.1 3666.2l17.6-18.4-11.2-6.5-17.5 18.5z"/>
      <path class="st30" d="M1494 3659.8c0 3.5 2.6 7.9 5.6 9.6 3 1.8 5.5.3 5.5-3.2l-11.1-6.4z"/>
      <path class="st29" d="M1527.2 3679l17.5-18.5-11-6.4-17.6 18.5z"/>
      <path class="st31" d="M1505.1 3666.2c0 3.5 2.4 7.8 5.5 9.6 3 1.8 5.5.3 5.5-3.2l-11-6.4z"/>
      <path class="st11" d="M1516.1 3672.6l17.6-18.5-11-6.3-17.6 18.4z"/>
      <path class="st30" d="M1516.1 3672.6c0 3.5 2.4 7.8 5.5 9.6 3 1.8 5.5.3 5.5-3.2l-11-6.4z"/>
      <path class="st11" d="M1538.2 3685.4l17.5-18.5-11-6.4-17.5 18.5z"/>
      <path class="st31" d="M1527.2 3679c0 3.5 2.4 7.8 5.5 9.6 3 1.8 5.5.4 5.5-3.2l-11-6.4z"/>
      <path class="st29" d="M1549.2 3691.8l17.6-18.5-11.1-6.4-17.5 18.5z"/>
      <path class="st30" d="M1538.2 3685.4c0 3.5 2.5 7.8 5.5 9.6 3 1.8 5.5.3 5.5-3.2l-11-6.4z"/>
      <path class="st23" d="M1480 3675.8l-6.7-3.8v3.4l6.7 3.8zm0 8.1l-6.7-3.9v3.4l6.7 3.9zm-4-6.3l-6.7-3.9v3.4l6.7 3.9zm85.2 52.7l-6.7-3.8v3.4l6.7 3.8zm-23.1-17.8l-6.7-3.9v3.4l6.7 3.9zm9.9 1l-6.7-3.9v3.4l6.7 3.9zm16.6 14.8l-6.7-3.8v3.4l6.7 3.8zm-7.4-4.3l-6.7-3.9v3.4l6.7 3.9z"/>
      <g class="st14">
        <path class="st29" d="M1512.9 3585.7c-3.6-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-1.9-15.2 1.5l10.9 6.4c5.9-3.5 11.3-3.8 15.2-1.5z"/>
        <path class="st29" d="M1497.7 3587.2l-10.9-6.4c-11.8 6.8-21.3 23.4-21.3 37l10.9 6.4c-.1-13.6 9.5-30.2 21.3-37z"/>
        <path class="st29" d="M1497.7 3587.2c-11.8 6.8-21.3 23.4-21.3 37l42.7-24.8c0-13.6-9.6-19.1-21.4-12.2z"/>
      </g>
      <g class="st14">
        <path class="st11" d="M1523.9 3592c-3.6-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-2-15.2 1.5l10.9 6.4c5.9-3.4 11.3-3.7 15.2-1.5z"/>
        <path class="st11" d="M1508.7 3593.5l-10.9-6.4c-11.8 6.8-21.3 23.4-21.3 37.1l10.9 6.4c-.1-13.6 9.5-30.2 21.3-37.1z"/>
        <path class="st11" d="M1508.7 3593.5c-11.8 6.8-21.3 23.4-21.3 37.1l42.7-24.8c0-13.6-9.6-19.1-21.4-12.3z"/>
      </g>
      <g class="st14">
        <path class="st29" d="M1534.8 3598.4c-3.6-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-2-15.2 1.5l10.9 6.4c5.9-3.4 11.3-3.8 15.2-1.5z"/>
        <path class="st29" d="M1519.6 3599.9l-10.9-6.4c-11.8 6.8-21.3 23.4-21.3 37.1l10.9 6.4c0-13.7 9.5-30.3 21.3-37.1z"/>
        <path class="st29" d="M1519.6 3599.9c-11.8 6.8-21.3 23.4-21.3 37.1l42.7-24.8c0-13.6-9.6-19.2-21.4-12.3z"/>
      </g>
      <g class="st14">
        <path class="st11" d="M1545.8 3604.8c-3.7-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-1.9-15.2 1.5l10.9 6.4c5.9-3.5 11.3-3.8 15.2-1.5z"/>
        <path class="st11" d="M1530.6 3606.3l-10.9-6.4c-11.8 6.8-21.3 23.4-21.3 37l11.1 6.5c-.1-13.6 9.2-30.3 21.1-37.1z"/>
        <path class="st29" d="M1530.6 3606.3c-11.8 6.8-21.2 23.6-21.1 37.2l42.5-24.9c0-13.7-9.6-19.2-21.4-12.3z"/>
      </g>
      <g class="st14">
        <path class="st29" d="M1556.7 3611.2c-3.6-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-1.9-15.2 1.5l10.9 6.4c5.9-3.5 11.3-3.8 15.2-1.5z"/>
        <path class="st29" d="M1541.5 3612.7l-10.9-6.4c-11.8 6.8-21.2 23.6-21.1 37.2l10.9 6.4c-.1-13.7 9.3-30.4 21.1-37.2z"/>
        <path class="st29" d="M1541.5 3612.7c-11.8 6.8-21.2 23.6-21.1 37.2l42.5-24.9c0-13.7-9.6-19.2-21.4-12.3z"/>
      </g>
      <g class="st14">
        <path class="st11" d="M1567.6 3617.5c-3.6-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-1.9-15.2 1.5l10.9 6.4c6-3.4 11.4-3.7 15.2-1.5z"/>
        <path class="st11" d="M1552.4 3619l-10.9-6.4c-11.8 6.8-21.2 23.6-21.1 37.2l11.2 6.5c-.1-13.5 9-30.4 20.8-37.3z"/>
        <path class="st11" d="M1552.4 3619c-11.8 6.8-20.9 23.7-20.9 37.3l42.3-25.1c0-13.5-9.6-19-21.4-12.2z"/>
      </g>
      <g class="st14">
        <path class="st29" d="M1578.6 3623.9c-3.7-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-2-15.2 1.5l10.9 6.4c5.9-3.4 11.3-3.8 15.2-1.5z"/>
        <path class="st29" d="M1563.4 3625.4l-10.9-6.4c-11.8 6.8-20.9 23.7-20.9 37.3l10.9 6.4c0-13.6 9.1-30.4 20.9-37.3z"/>
        <path class="st29" d="M1563.4 3625.4c-11.8 6.8-20.9 23.7-20.9 37.3l42.3-25.1c0-13.5-9.6-19-21.4-12.2z"/>
      </g>
      <g class="st14">
        <path class="st11" d="M1589.5 3630.3c-3.7-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-1.9-15.2 1.5l10.9 6.4c6-3.5 11.4-3.8 15.2-1.5z"/>
        <path class="st11" d="M1574.3 3631.8l-10.9-6.4c-11.8 6.8-20.9 23.7-20.9 37.3l11 6.5c0-13.6 9-30.6 20.8-37.4z"/>
        <path class="st29" d="M1574.3 3631.8c-11.8 6.8-20.8 23.8-20.8 37.4l42.2-25.1c0-13.7-9.6-19.2-21.4-12.3z"/>
      </g>
      <path class="st29" d="M1600.5 3636.7c-3.6-2.1-7.3-4.3-10.9-6.4-3.9-2.3-9.3-2-15.2 1.5l10.9 6.4c5.9-3.5 11.3-3.8 15.2-1.5z"/>
      <path class="st29" d="M1585.3 3638.2l-10.9-6.4c-11.8 6.8-20.8 23.8-20.8 37.4l11.2 6.4c-.1-13.6 8.7-30.6 20.5-37.4z"/>
      <path class="st32" d="M1585.3 3638.2c-11.8 6.8-20.6 23.8-20.6 37.4l42-25.1c0-13.7-9.6-19.2-21.4-12.3z"/>
    </g>
    <g id="greek-building">
      <path class="st16" d="M1613.7 2525l1.3-.7-58.5-34-58.8 34 16.6 9.6-8.9 5.2 1.9 1.1-3.4 2 2.2 1.3-3.6 2.1 73.1 42.5 73.5-42.5z"/>
      <path class="st33" d="M1506.5 2543.6l.1 4.6 73.1 42.5-.1-4.6z"/>
      <path class="st34" d="M1579.6 2586.1l.1 4.6 73.5-42.5v-4.6z"/>
      <path class="st29" d="M1506.5 2543.6l73.1 42.5 73.6-42.5-73.1-42.4z"/>
      <path class="st33" d="M1513.9 2538.5v4.7l65.8 38.2v-4.6z"/>
      <path class="st34" d="M1579.7 2576.8v4.6l66.2-38.2v-4.7z"/>
      <path class="st29" d="M1513.9 2538.5l65.8 38.3 66.2-38.3-65.8-38.2z"/>
      <path class="st33" d="M1521.2 2532.2l.1 4.6 58.4 34v-4.7z"/>
      <path class="st34" d="M1579.7 2566.1v4.7l58.8-34v-4.6z"/>
      <path class="st35" d="M1521.2 2532.2l58.5 33.9 58.8-33.9-58.5-34z"/>
      <path class="st29" d="M1616.4 2533.9l10.8-5.9-50.5-28-9.2 5.3zm-21.7 12l10.3-6.9-49.3-26.8-9.4 5.4zM1574 2558l13.7-5.2-52.7-28.6-9.4 5.5z"/>
      <g class="st14">
        <path class="st36" d="M1530.2 2489.8l.1 40.3c0 1.2.8 2.4 2.3 3.3 3.1 1.8 8.2 1.8 11.3 0 1.6-.9 2.4-2.1 2.4-3.3l-.1-40.3c0 1.2-.8 2.4-2.4 3.3-3.1 1.8-8.2 1.8-11.3 0-1.6-.9-2.3-2.1-2.3-3.3z"/>
        <path class="st21" d="M1541.6 2494c.8-.2 1.6-.5 2.2-.9 1.6-.9 2.4-2.1 2.4-3.3l.1 40.3c0 1.2-.8 2.4-2.4 3.3-.7.4-1.5.7-2.3.9V2494z"/>
        <path class="st29" d="M1532.5 2486.5c-3.1 1.8-3.2 4.7 0 6.6 3.1 1.8 8.2 1.8 11.3 0 3.1-1.8 3.1-4.7 0-6.6-3.1-1.8-8.1-1.8-11.3 0z"/>
      </g>
      <g class="st14">
        <path class="st33" d="M1530.1 2496.2l11.7-6.8c.6-.4 1-1.1 1-2.2l-11.7 6.8c0 1.1-.4 1.8-1 2.2z"/>
        <path class="st29" d="M1537 2481.1l-11.7 6.8c.6-.4 1.5-.3 2.4.2l11.7-6.8c-.9-.5-1.7-.6-2.4-.2zm0 12.4l11.7-6.9-9.2-5.3-11.8 6.8z"/>
        <path class="st29" d="M1539.4 2501.5l11.7-6.8c.6-.4 1-1.1 1-2.2 0-2.2-1.5-4.8-3.4-5.9l-11.7 6.8c1.9 1.1 3.4 3.7 3.4 5.9-.1 1.1-.4 1.9-1 2.2z"/>
        <path class="st33" d="M1527.7 2488.1c-1.9-1.1-3.4-.2-3.4 1.9 0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2l2.4 1.4c0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2s-1.5-4.8-3.4-5.9l-9.2-5.2z"/>
      </g>
      <g class="st14">
        <path class="st36" d="M1613.9 2489.8l.1 40.3c0 1.2.8 2.4 2.3 3.3 3.1 1.8 8.2 1.8 11.3 0 1.6-.9 2.4-2.1 2.4-3.3l-.1-40.3c0 1.2-.8 2.4-2.4 3.3-3.1 1.8-8.2 1.8-11.3 0-1.5-.9-2.3-2.1-2.3-3.3z"/>
        <path class="st21" d="M1625.3 2494c.8-.2 1.6-.5 2.2-.9 1.6-.9 2.4-2.1 2.4-3.3l.1 40.3c0 1.2-.8 2.4-2.4 3.3-.7.4-1.5.7-2.3.9V2494z"/>
        <path class="st29" d="M1616.3 2486.5c-3.1 1.8-3.1 4.7 0 6.6 3.1 1.8 8.2 1.8 11.3 0 3.1-1.8 3.2-4.7 0-6.6-3.1-1.8-8.2-1.8-11.3 0z"/>
      </g>
      <g class="st14">
        <path class="st33" d="M1613.9 2496.2l11.7-6.8c.6-.4 1-1.1 1-2.2l-11.7 6.8c0 1.1-.4 1.8-1 2.2zm6.9-15.1l-11.7 6.8c.6-.4 1.5-.3 2.4.2l11.7-6.8c-.9-.5-1.8-.6-2.4-.2z"/>
        <path class="st33" d="M1620.7 2493.5l11.7-6.9-9.2-5.3-11.7 6.8z"/>
        <path class="st29" d="M1623.1 2501.5l11.7-6.8c.6-.4 1-1.1 1-2.2 0-2.2-1.5-4.8-3.4-5.9l-11.7 6.8c1.9 1.1 3.4 3.7 3.4 5.9 0 1.1-.4 1.9-1 2.2z"/>
        <path class="st29" d="M1611.5 2488.1c-1.9-1.1-3.4-.2-3.4 1.9 0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2l2.4 1.4c0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2s-1.5-4.8-3.4-5.9l-9.2-5.2z"/>
      </g>
      <g class="st14">
        <path class="st36" d="M1551.4 2502.1l.1 40.3c0 1.2.8 2.4 2.3 3.3 3.1 1.8 8.2 1.8 11.3 0 1.6-.9 2.4-2.1 2.4-3.3l-.1-40.3c0 1.2-.8 2.4-2.4 3.3-3.1 1.8-8.2 1.8-11.3 0-1.6-1-2.3-2.2-2.3-3.3z"/>
        <path class="st21" d="M1562.8 2506.2c.8-.2 1.6-.5 2.2-.9 1.6-.9 2.4-2.1 2.4-3.3l.1 40.3c0 1.2-.8 2.4-2.4 3.3-.7.4-1.5.7-2.3.9v-40.3z"/>
        <path class="st29" d="M1553.7 2498.8c-3.1 1.8-3.1 4.8 0 6.6 3.1 1.8 8.2 1.8 11.3 0 3.1-1.8 3.1-4.7 0-6.5-3.1-1.9-8.1-1.9-11.3-.1z"/>
      </g>
      <g class="st14">
        <path class="st33" d="M1551.3 2508.4l11.7-6.8c.6-.4 1-1.1 1-2.2l-11.7 6.8c0 1.1-.4 1.9-1 2.2z"/>
        <path class="st29" d="M1558.2 2493.3l-11.7 6.8c.6-.4 1.5-.3 2.4.2l11.7-6.8c-.9-.5-1.8-.6-2.4-.2zm-.1 12.4l11.8-6.8-9.2-5.3-11.8 6.8z"/>
        <path class="st29" d="M1560.5 2513.8l11.7-6.8c.6-.4 1-1.1 1-2.2 0-2.2-1.5-4.8-3.4-5.9l-11.7 6.8c1.9 1.1 3.4 3.7 3.4 5.9 0 1.1-.3 1.8-1 2.2z"/>
        <path class="st33" d="M1548.9 2500.4c-1.9-1.1-3.4-.2-3.4 1.9 0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2l2.4 1.4c0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2s-1.5-4.8-3.4-5.9l-9.2-5.2z"/>
      </g>
      <path class="st36" d="M1593.7 2502.1l.1 40.3c0 1.2.8 2.4 2.3 3.3 3.1 1.8 8.2 1.8 11.3 0 1.6-.9 2.4-2.1 2.4-3.3l-.1-40.3c0 1.2-.8 2.4-2.4 3.3-3.1 1.8-8.2 1.8-11.3 0-1.6-1-2.3-2.2-2.3-3.3z"/>
      <path class="st21" d="M1605.1 2506.2c.8-.2 1.6-.5 2.2-.9 1.6-.9 2.4-2.1 2.4-3.3l.1 40.3c0 1.2-.8 2.4-2.4 3.3-.7.4-1.5.7-2.3.9v-40.3z"/>
      <path class="st29" d="M1596 2498.8c-3.1 1.8-3.1 4.8 0 6.6 3.1 1.8 8.2 1.8 11.3 0 3.1-1.8 3.2-4.7 0-6.5-3.1-1.9-8.2-1.9-11.3-.1z"/>
      <g class="st14">
        <path class="st33" d="M1593.6 2508.4l11.7-6.8c.6-.4 1-1.1 1-2.2l-11.7 6.8c0 1.1-.4 1.9-1 2.2zm6.9-15.1l-11.7 6.8c.6-.4 1.5-.3 2.4.2l11.7-6.8c-.9-.5-1.8-.6-2.4-.2z"/>
        <path class="st33" d="M1600.4 2505.7l11.8-6.8-9.3-5.3-11.7 6.8z"/>
        <path class="st29" d="M1602.8 2513.8l11.7-6.8c.6-.4 1-1.1 1-2.2 0-2.2-1.5-4.8-3.4-5.9l-11.7 6.8c1.9 1.1 3.4 3.7 3.4 5.9 0 1.1-.3 1.8-1 2.2z"/>
        <path class="st29" d="M1591.2 2500.4c-1.9-1.1-3.4-.2-3.4 1.9 0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2l2.4 1.4c0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2s-1.5-4.8-3.4-5.9l-9.2-5.2z"/>
      </g>
      <g class="st14">
        <path class="st36" d="M1571.8 2514.3l.1 40.3c0 1.2.8 2.4 2.3 3.3 3.1 1.8 8.2 1.8 11.3 0 1.6-.9 2.4-2.1 2.4-3.3l-.1-40.3c0 1.2-.8 2.4-2.4 3.3-3.1 1.8-8.2 1.8-11.3 0-1.5-.9-2.3-2.1-2.3-3.3z"/>
        <path class="st21" d="M1583.2 2518.5c.8-.2 1.6-.5 2.2-.9 1.6-.9 2.4-2.1 2.4-3.3l.1 40.3c0 1.2-.8 2.4-2.4 3.3-.7.4-1.5.7-2.3.9v-40.3z"/>
        <path class="st29" d="M1574.2 2511c-3.1 1.8-3.1 4.7 0 6.6 3.1 1.8 8.2 1.8 11.3 0 3.1-1.8 3.2-4.7 0-6.5-3.1-1.9-8.2-1.9-11.3-.1z"/>
      </g>
      <g class="st14">
        <path class="st33" d="M1571.8 2520.7l11.7-6.8c.6-.4 1-1.1 1-2.2l-11.7 6.8c0 1.1-.4 1.8-1 2.2z"/>
        <path class="st29" d="M1578.7 2505.6l-11.7 6.8c.6-.4 1.5-.3 2.4.2l11.7-6.8c-.9-.6-1.8-.6-2.4-.2z"/>
        <path class="st29" d="M1578.6 2518l11.8-6.9-9.3-5.3-11.7 6.8z"/>
        <path class="st29" d="M1581 2526l11.7-6.8c.6-.4 1-1.1 1-2.2 0-2.2-1.5-4.8-3.4-5.9l-11.7 6.8c1.9 1.1 3.4 3.7 3.4 5.9 0 1.1-.4 1.9-1 2.2z"/>
        <path class="st33" d="M1569.4 2512.6c-1.9-1.1-3.4-.2-3.4 1.9 0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-1.9l2.4 1.4c0 2.2 1.5 4.8 3.4 5.9 1.9 1.1 3.4.2 3.4-2s-1.5-4.8-3.4-5.9l-9.2-5.3z"/>
      </g>
      <path class="st11" d="M1554.6 2479.9c-.5-.3-.9-.4-1.3-.3l-20.6 4.9c-.7.1-.7 1.1 0 2.1l43.7 25.3c.7-.2.7-1.2 0-2.1l-20.5-28.6c-.3-.6-.8-1-1.3-1.3z"/>
      <path class="st33" d="M1552.8 2474.9c.5-.1 1.2.1 1.8.4.7.4 1.3 1 1.8 1.7l28.3 39.4c1 1.4 1 2.7 0 2.9l-60.3-34.8c-.9-1.4-.9-2.7 0-2.9l28.4-6.7zm-20.1 11.7l43.7 25.3c.7-.2.7-1.2 0-2.1l-20.5-28.6c-.4-.5-.8-.9-1.3-1.2-.5-.3-.9-.4-1.3-.3l-20.6 4.9c-.7.1-.7 1 0 2z"/>
      <path class="st37" d="M1604.4 2446.4c-.6-.4-1.3-.5-1.8-.4l-28.4 6.7-49.8 28.9 28.4-6.7c.5-.1 1.1.1 1.7.4l50.6-28.4c-.2-.2-.4-.3-.7-.5z"/>
      <path class="st38" d="M1634.5 2487.6l-28.3-39.4c-.3-.5-.7-.9-1.2-1.2l-50.6 28.4s.1 0 .1.1c.7.4 1.3 1 1.8 1.7l28.3 39.4c.9 1.2 1 2.4.3 2.8l49.8-28.9c.8-.5.7-1.7-.2-2.9z"/>
    </g>
    <path class="st11" d="M1839.8 414.5c-19.4-11.2-36.1-7.7-44 6.6-7.2-9-15.5-16.7-24.4-21.9-19.6-11.3-36.4-7.7-44.3 7-1.5-1.1-3.1-2.3-4.6-3.2-27-15.6-48.9-3.1-49 27.9-.1 31 21.7 68.8 48.7 84.3l187 107.9c27 15.6 48.9 3 49-28 .1-31-21.7-68.7-48.7-84.3-7.8-4.5-14.9-6.4-21.5-6.5.2-1.9.5-3.6.5-5.6.1-30.9-21.7-68.6-48.7-84.2z" id="cloud-1"/>
    <path class="st11" d="M1913.8 3646.6c-18.8-10.8-34.9-7.4-42.5 6.4-7-8.7-15-16.2-23.6-21.2-18.9-10.9-35.2-7.4-42.8 6.7-1.5-1.1-2.9-2.2-4.5-3.1-26.1-15.1-47.3-3-47.4 27-.1 30 21 66.4 47.1 81.5l180.7 104.3c26.1 15 47.3 2.9 47.3-27 .1-30-21-66.4-47-81.4-7.5-4.3-14.4-6.2-20.7-6.3.2-1.8.5-3.5.5-5.4 0-29.9-21-66.4-47.1-81.5z" id="cloud-2"/>
    <path class="st11" d="M1037.2 90c10.9-6.3 20.2-4.3 24.6 3.7 4-5.1 8.7-9.4 13.7-12.3 11-6.4 20.4-4.3 24.8 3.9.9-.6 1.7-1.3 2.6-1.8 15.1-8.8 27.4-1.7 27.4 15.7s-12.1 38.7-27.3 47.4l-104.7 60.7c-15.1 8.8-27.4 1.7-27.4-15.7s12.1-38.6 27.3-47.4c4.3-2.5 8.4-3.6 12-3.6-.1-1-.3-2-.3-3.1 0-17.5 12.2-38.8 27.3-47.5z" id="cloud-3"/>
    <path class="st11" d="M850.4 162.9c6.3-3.6 11.6-2.5 14.2 2.1 2.3-2.9 5-5.4 7.9-7.1 6.3-3.7 11.7-2.5 14.3 2.3.5-.4 1-.7 1.5-1 8.7-5 15.8-1 15.8 9s-7 22.3-15.7 27.3l-60.3 35c-8.7 5-15.8 1-15.8-9.1 0-10 7-22.3 15.7-27.3 2.5-1.5 4.8-2.1 6.9-2.1-.1-.6-.2-1.2-.2-1.8 0-10.1 7-22.3 15.7-27.3z" id="cloud-4"/>
    <path class="st11" d="M757.5 685.2c6.3-3.6 11.6-2.5 14.2 2.1 2.3-2.9 5-5.4 7.9-7.1 6.3-3.7 11.7-2.5 14.3 2.3.5-.4 1-.7 1.5-1 8.7-5 15.8-1 15.8 9s-7 22.3-15.7 27.3l-60.3 35c-8.7 5-15.8 1-15.8-9.1 0-10 7-22.3 15.7-27.3 2.5-1.5 4.8-2.1 6.9-2.1-.1-.6-.2-1.2-.2-1.8-.1-10 7-22.2 15.7-27.3z" id="cloud-5"/>
    <path class="st11" d="M255.5 589.5c7-4.1 13-2.8 15.8 2.4 2.6-3.3 5.6-6.1 8.8-7.9 7.1-4.1 13.1-2.8 15.9 2.5.6-.4 1.1-.8 1.7-1.2 9.7-5.6 17.6-1.1 17.6 10.1s-7.8 24.9-17.5 30.5l-67.3 39c-9.7 5.6-17.6 1.1-17.6-10.1s7.8-24.8 17.5-30.5c2.8-1.6 5.4-2.3 7.7-2.3-.1-.7-.2-1.3-.2-2 0-11.2 7.8-24.8 17.6-30.5z" id="cloud-6"/>
    <path class="st11" d="M2 1989.6c12.4-7.2 23.1-4.9 28.2 4.3 4.6-5.8 9.9-10.8 15.6-14.1 12.5-7.3 23.3-4.9 28.3 4.5 1-.7 2-1.5 3-2.1 17.3-10 31.3-2 31.4 17.9.1 19.9-13.9 44.2-31.2 54.2l-119.6 69.4c-17.3 10-31.3 2-31.3-18-.1-19.9 13.9-44.2 31.1-54.2 5-2.9 9.6-4.1 13.7-4.2-.1-1.2-.3-2.3-.3-3.6-.1-19.9 13.9-44.1 31.1-54.1z" id="cloud-7"/>
    <path class="st11" d="M403 2963.5c12.4-7.2 23.1-4.9 28.2 4.3 4.6-5.8 9.9-10.8 15.6-14.1 12.5-7.3 23.3-4.9 28.3 4.5 1-.7 2-1.5 3-2.1 17.3-10 31.3-2 31.4 17.9.1 19.9-13.9 44.2-31.2 54.2l-119.6 69.4c-17.3 10-31.3 2-31.3-18-.1-19.9 13.9-44.2 31.1-54.2 5-2.9 9.6-4.1 13.7-4.2-.1-1.2-.3-2.3-.3-3.6-.1-19.9 13.9-44.1 31.1-54.1z" id="cloud-8"/>
    <path class="st11" d="M196.2 3045c6.6-3.8 12.2-2.6 14.9 2.2 2.4-3.1 5.2-5.7 8.3-7.4 6.6-3.8 12.3-2.6 15 2.4.5-.4 1-.8 1.6-1.1 9.1-5.3 16.5-1.1 16.6 9.5 0 10.5-7.3 23.3-16.4 28.6l-63.1 36.6c-9.1 5.3-16.5 1-16.5-9.5s7.3-23.3 16.4-28.6c2.6-1.5 5-2.2 7.2-2.2-.1-.6-.2-1.2-.2-1.9-.2-10.5 7.1-23.3 16.2-28.6z" id="cloud-9"/>
    <path class="st11" d="M144.2 3603.3c9.8-5.7 18.1-3.9 22.1 3.3 3.6-4.6 7.8-8.5 12.3-11.1 9.9-5.7 18.3-3.9 22.3 3.5.8-.6 1.5-1.2 2.3-1.6 13.6-7.9 24.6-1.6 24.6 14.1 0 15.6-10.9 34.7-24.5 42.6l-94 54.5c-13.6 7.9-24.6 1.5-24.6-14.1s10.9-34.7 24.5-42.5c3.9-2.3 7.5-3.2 10.8-3.3-.1-.9-.3-1.8-.3-2.8 0-15.7 10.9-34.8 24.5-42.6z" id="cloud-10"/>
    <g id="round-tree-3">
      <path class="st16" d="M766.7 331.8c-.1.3-.7.7-1.2.8h-.2c-.2 0-.4 0-.6-.1l-8.8-5.2c-.2.6-.6 1.1-1.4 1.5-1.9 1.2-5.1 1.2-7.1 0-1.8-1.1-1.9-2.8-.4-3.9-.5-.1-.9-.3-1.3-.5-2-1.2-2-3 0-4.2 1.9-1.2 5.1-1.2 7 0 .4.2.7.5.9.8 1.9-.9 4.8-.9 6.6.2 1.4.9 1.8 2.1 1.2 3.1.3.1.6.2.8.3.8.5.8 1.3 0 1.8-.2.1-.5.2-.7.3v1.8l5 3c.2 0 .2.1.2.3zm-9-5.6l2.2 1.3v-.8c-.2-.1-.5-.2-.7-.3-.2-.1-.3-.3-.5-.4-.2 0-.6.1-1 .2z"/>
      <path class="st17" d="M766.5 331.1c.7.4.8 1.1 0 1.6-.7.4-1.8.4-2.5.1-.1 0-.1-.1-.2-.1s-.1-.1-.2-.1c-.6-.4-.5-1.1.1-1.5.9-.4 2.1-.4 2.8 0z"/>
      <path class="st18" d="M771.7 303c.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9-3.8 0-6.9 3.1-6.9 6.9 0 .7.1 1.4.3 2.1-3.4.4-6.1 3.3-6.1 6.8 0 3.8 3.1 6.9 6.9 6.9 2.4 0 4.5-1.2 5.7-3.1 1.2 1.9 3.3 3.1 5.7 3.1 3.8 0 6.9-3.1 6.9-6.9.2-3.5-2.4-6.4-5.9-6.8z"/>
      <path class="st19" d="M770.9 316.7c3.8 0 6.9-3.1 6.9-6.9 0-3.5-2.7-6.4-6.1-6.8.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9v19.6c1.3 1.9 3.4 3.1 5.8 3.1z"/>
      <path class="st17" d="M763.3 297.7h3.8v34.2h-3.8z"/>
      <path class="st18" d="M771.7 289.9c.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9-3.8 0-6.9 3.1-6.9 6.9 0 .7.1 1.4.3 2.1-3.4.4-6.1 3.3-6.1 6.8 0 3.8 3.1 6.9 6.9 6.9 2.4 0 4.5-1.2 5.7-3.1 1.2 1.9 3.3 3.1 5.7 3.1 3.8 0 6.9-3.1 6.9-6.9.2-3.5-2.4-6.4-5.9-6.8z"/>
      <path class="st19" d="M770.9 303.6c3.8 0 6.9-3.1 6.9-6.9 0-3.5-2.7-6.4-6.1-6.8.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9v19.6c1.3 1.9 3.4 3.1 5.8 3.1z"/>
      <circle class="st18" cx="771.2" cy="304.3" r="2.9"/>
      <path class="st17" d="M765.2 311.3c-.3 0-.6-.1-.8-.3-.4-.4-.4-1.1 0-1.6l5.9-5.9c.4-.4 1.1-.4 1.6 0 .4.4.4 1.1 0 1.6L766 311c-.2.2-.5.3-.8.3z"/>
      <circle class="st18" cx="770.6" cy="315.1" r="2.3"/>
      <path class="st17" d="M765.9 320.7c-.2 0-.4-.1-.6-.3-.3-.3-.3-.9 0-1.2l4.6-4.6c.3-.3.9-.3 1.2 0 .3.3.3.9 0 1.2l-4.6 4.6c-.1.2-.3.3-.6.3z"/>
      <circle class="st19" cx="758.2" cy="309.3" r="3.4"/>
      <path class="st17" d="M765.1 317.5c.3 0 .7-.1.9-.4.5-.5.5-1.3 0-1.8l-6.7-6.7c-.5-.5-1.3-.5-1.8 0s-.5 1.3 0 1.8l6.7 6.7c.3.3.6.4.9.4z"/>
    </g>
    <g id="school">
      <path class="st39 st40" d="M365.7 466.1l6.2 3.6 68.5 37 87.5 36.4L761 408.5l-69.9-40.3-84.4-44.2-197.2 115.3z"/>
      <g class="st14">
        <path class="st41" d="M528.1 531l-98.7-57.8.1 10 98.7 57.8z"/>
        <path class="st42" d="M759.8 397.3l-98.7-57.8-231.7 133.7 98.7 57.8z"/>
        <path class="st43" d="M759.8 397.3L528.1 531l.1 10 231.6-133.7z"/>
      </g>
      <path class="st44 st45" d="M527.4 520.1l-82.9-55.6-15 8.7 68.8 40.4z"/>
      <g class="st14">
        <path class="st46" d="M745.3 330.2l-84.1-48.9-48 27.7 84.2 48.9z"/>
        <path class="st47" d="M666.7 284.8v-7.5l-31.3 18 6.7 3.8z"/>
        <path class="st48" d="M575.7 393.5l-84.1-48.9.1 34.6 84.1 48.9z"/>
        <path class="st6" d="M697.3 323.3l-84.1-48.8-121.6 70.1 84.1 48.9z"/>
        <path class="st46" d="M575.8 428.1l-84.1-48.9-48 27.7 84.1 48.9z"/>
        <path class="st48" d="M527.8 455.8l-84.1-48.9.2 64.8 84.1 48.9z"/>
        <path class="st49" d="M528 520.6l48-27.7 67-38.7-.6-23.1 21.7 10.9 33.4-19.3 48-27.7-.2-64.8-47.9 27.7-.1-34.6-121.6 70.2.1 34.6-48 27.7z"/>
      </g>
      <path class="st48" d="M662.1 411.6h-17.9v20.5l19.9 9.9-.1-12.9z"/>
      <g class="st14">
        <path class="st6" d="M491.7 372l-48 27.7 5.5 3.2 48-27.7z"/>
        <path class="st47" d="M497.2 375.2l-48 27.7v7.5l48-27.6z"/>
      </g>
      <path class="st50" d="M588.9 432.1l3.1-1.8 9.2-5.3 1.1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v20zm17.6-10.1l3.1-1.7 9.2-5.4 1-.6v-23.6l-3.1 1.8-9.2 5.3-1.1.6v1.2l.1 18.9zm17.7-9.9l3.1-1.8 9.2-5.3 1.1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v20zm17.6-10.1l3.1-1.7 9.2-5.4 1.1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1.1.6v1.2l.1 18.9zm16-9.7l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8V361l-3.1 1.8-9.2 5.3-1 .6v20.1zm17.5-10l3.1-1.8 9.2-5.3 1.1-.6v-1.2l-.1-18.9V351l-3.1 1.7-9.2 5.4-1 .6v20zM537.7 501.5l3.1-1.7 9.2-5.4 1-.6v-23.6l-3.1 1.8-9.3 5.3-1 .6v1.2l.1 18.9zm-20.8-4v-3.2l-13.3-7.7-.1 3.2 1.1.6 9.2 5.3zm-17.6-9.9l.1-3.3-13.4-7.7v3.3l1 .6 9.2 5.3zm-15.9-9.9v-3.3l-13.3-7.7-.1 3.3 1.1.6 9.2 5.3zm-17.5-9.8v-3.2l-13.3-7.7-.1 3.2 1.1.6 9.2 5.3zm89.5 23.7l3.1-1.8 9.2-5.3 1.1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v20zm17.6-10.1l3.1-1.7 9.2-5.4 1-.6v-23.6l-3.1 1.8-9.2 5.3-1.1.6v1.2l.1 18.9zm15.9-9.7l3.1-1.8 9.2-5.3 1.1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v20.1zm86.2-48.5l3.1-1.8 9.2-5.3 1-.6v-20.1l-.1-3.6-3.1 1.8-9.2 5.4-1 .6v1.2l.1 18.8zm17.5-10.1l3.1-1.8 9.2-5.3 1.1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v20zm16-9.7l3.1-1.8 9.2-5.3 1-.6v-23.6l-3.1 1.8-9.2 5.3-1.1.6v1.2l.1 18.8zm17.6-10.1l3-1.7 9.3-5.4 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v20.1z"/>
      <g class="st14">
        <path class="st51" d="M601.2 399.8l-11.3 6.5.1 21.2 11.2-6.5z"/>
        <path class="st11" d="M588.9 429.3l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8V398l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.7l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M618.7 389.8l-11.2 6.5v21.2l11.3-6.5z"/>
        <path class="st11" d="M606.5 419.3l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8V388l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.8l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M636.5 379.8l-11.3 6.5.1 21.2 11.2-6.5z"/>
        <path class="st11" d="M624.2 409.3l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8V378l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.3-27.7l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M654.1 369.8l-11.3 6.5v21.2l11.3-6.5z"/>
        <path class="st11" d="M641.8 399.3l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8V368l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.8l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M670 360l-11.3 6.6.1 21.2 11.3-6.5z"/>
        <path class="st11" d="M657.8 389.6l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.8l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M687.6 350l-11.3 6.5.1 21.2 11.2-6.5z"/>
        <path class="st11" d="M675.3 379.5l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.7l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M549.9 469.3l-11.3 6.5.1 21.2 11.3-6.5z"/>
        <path class="st11" d="M537.7 498.8l3.1-1.8 9.2-5.3 1-.6v-23.7l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8-.1 3.7zm11.2-27.8l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M567.7 459.3l-11.3 6.5v21.3l11.3-6.6z"/>
        <path class="st11" d="M555.4 488.8l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.7l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M585.2 449.3l-11.2 6.5V477l11.3-6.5z"/>
        <path class="st11" d="M573 478.8l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.8l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M601.2 439.5l-11.3 6.6.1 21.2 11.2-6.5z"/>
        <path class="st11" d="M588.9 469.1l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.8l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st52" d="M505.7 466.6v18.8l9.2 5.3v-18.8z"/>
        <path class="st39 st49" d="M516.9 494.3v-3.6l.1-18.8v-1.2l-1-.6-9.2-5.3-3.1-1.8v3.6l-.1 18.8v1.2l1 .6 9.2 5.3 3.1 1.8zm-11.2-27.7l9.2 5.3-.1 18.8-9.2-5.3.1-18.8z"/>
      </g>
      <g class="st14">
        <path class="st52" d="M488.2 456.5v18.8l9.1 5.4.1-18.9z"/>
        <path class="st39 st49" d="M499.4 484.3v-3.6l.1-18.8v-1.2l-1-.6-9.2-5.3-3.1-1.8v23.6l1 .6 9.2 5.3 3 1.8zm-11.2-27.8l9.2 5.3-.1 18.8-9.2-5.3v-18.8z"/>
      </g>
      <g class="st14">
        <path class="st52" d="M472.2 446.8v18.8l9.2 5.4v-18.9z"/>
        <path class="st39 st49" d="M483.4 474.5v-3.6l.1-18.8v-1.2l-1-.6-9.2-5.3-3.1-1.8v3.6l-.1 18.8v1.2l1 .6 9.2 5.3 3.1 1.8zm-11.2-27.7l9.2 5.3-.1 18.8-9.2-5.3.1-18.8z"/>
      </g>
      <g class="st14">
        <path class="st52" d="M454.7 436.7l-.1 18.9 9.2 5.3.1-18.8z"/>
        <path class="st39 st49" d="M465.9 464.5v-3.6l.1-18.8v-1.2l-1-.6-9.2-5.3-3.1-1.8v3.6l-.1 18.8v1.2l1 .6 9.2 5.3 3.1 1.8zm-11.2-27.8l9.2 5.3-.1 18.8-9.2-5.3.1-18.8z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M687.3 391l-11.3 6.5.1 21.2 11.3-6.5z"/>
        <path class="st11" d="M675.1 420.5l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.7l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M704.9 380.9l-11.3 6.5.1 21.3 11.2-6.6z"/>
        <path class="st11" d="M692.6 410.4l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.3-27.7l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M720.8 371.2l-11.2 6.5v21.2l11.3-6.5z"/>
        <path class="st11" d="M708.6 400.7l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.7l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st51" d="M738.4 361.2l-11.3 6.5.1 21.2 11.3-6.5z"/>
        <path class="st11" d="M726.2 390.7l3.1-1.8 9.2-5.3 1-.6v-1.2l-.1-18.8v-3.6l-3.1 1.8-9.2 5.3-1 .6v1.2l.1 18.8v3.6zm11.2-27.8l.1 18.8-9.2 5.3-.1-18.8 9.2-5.3z"/>
      </g>
      <g class="st14">
        <path class="st53" d="M527.9 448.2l-.1 7.6 5.5-3.2V445z"/>
        <path class="st6" d="M533.3 445l-78.6-45.3-5.4 3.2 78.6 45.3z"/>
      </g>
      <g class="st14">
        <path class="st54 st55" d="M491.8 354.7l84.1 48.8.1-7.5-7.3-4.5-3.8-2.2-73.1-42.1zm205.4-29L576 395.8v7.5l121.2-70z"/>
        <path class="st56" d="M449.2 402.9l-5.5-3.2.1 7.5 5.4 3.2zm0 7.5l78.6 45.4.1-7.6-1.8-1-3.7-2.2v.1l-73.1-42.2zm42.6-58.2l84.1 48.9.1-7.6-7.3-4.5-3.8-2.2v.1l-73.1-42.2z"/>
        <path class="st6" d="M570.3 417.3L522.4 445l5.4 3.2 48-27.6z"/>
        <path class="st47" d="M575.8 420.6l-48 27.6v7.6l48-27.7zm121.4-97.4L576 393.3v7.6l121.2-70.1z"/>
      </g>
      <path class="st14 st6" d="M661.2 274L630 292.1l5.4 3.2 31.3-18z"/>
      <g class="st14">
        <path class="st53" d="M739.8 325.9v7.5l5.4-3.2.1-7.6z"/>
        <path class="st47" d="M661.2 280.5l-.1 7.6 78.7 45.3v-7.5z"/>
        <path class="st6" d="M666.6 277.3l-5.7 3 78.9 45.6 5.5-3.3z"/>
      </g>
      <g class="st14">
        <path class="st6" d="M697.4 343.9l-.1 6.4 48-27.7-5.5-3.2z"/>
        <path class="st47" d="M745.3 322.6l-48 27.7.1 7.5 47.9-27.6z"/>
      </g>
      <g class="st14">
        <path class="st57" d="M663.2 403.5l-4.5 2.3 4.5 2.6 4.5-2.3z"/>
        <path class="st53" d="M663.2 408.4l-4.5-2.6.1 40.4 4.5 2.6z"/>
        <path class="st11" d="M667.7 406.1l-4.5 2.3.1 40.4 4.5-2.3z"/>
      </g>
      <g class="st14">
        <path class="st58 st59" d="M644.8 416.5v33.6l16.3-2.6-.1-40.4z"/>
        <path class="st60" d="M656.4 404.4l-16.1 9.4 4.5 2.6 16.1-9.4zm-16.1 9.4l-16 9.2 4.5 2.6 16-9.2z"/>
        <path class="st61" d="M628.8 425.6l-4.5-2.6.1 40.4 4.5 2.6z"/>
        <path class="st51" d="M643.7 418.2l-13.9 8 .1 38 13.8-8.1z"/>
        <path class="st62" d="M644.8 416.4l-16 9.2.1 40.4 15.9-9.3v-40.3zm-2.1 39.1l-11.7 6.9-.1-35.6 11.8-6.8v35.5z"/>
      </g>
      <g class="st14">
        <path class="st57" d="M625.9 423.9l-4.5 2.3 4.5 2.6 4.5-2.3z"/>
        <path class="st63" d="M621.5 426.2v40.4l4.4 2.6v-40.4z"/>
        <path class="st11" d="M625.9 428.8v40.4l4.6-2.3v-40.4z"/>
      </g>
      <g class="st14">
        <path class="st6" d="M661.2 401.3l-21.9 3.8 9.6 5.3 21.9-3.8z"/>
        <path class="st64" d="M639.3 405.1L616.6 427l9.6 5.3 22.7-21.9z"/>
        <path class="st11" d="M648.9 411.8l-22.7 20.5 44.6-25.7z"/>
      </g>
      <path class="st54 st55" d="M565.1 420.3l-1 .6 1-.6zm5.2-3l-5.2 3 10.7.3zM491.7 372l-21.9 12.4 9.9.9v7.2l81.6 30 2.8-1.6-.3.2-66.6-38.5v-7.4z"/>
      <path class="st54 st65" d="M625.9 436.5l42.2-28.2-41.8 24-9.7-5.3v42.5l9.3-.3v-31.7z"/>
      <path class="st66" d="M664 410.5l6.8-3.9-21.9 3.8-22.7 21.9 7.1-4 15.6-15.2z"/>
      <path class="st54 st55" d="M661.4 280.7l-5.2 10.3 67.7 37.6 10.3-5.8z"/>
      <path class="st46" d="M623.6 354.7L558 315.8l-48.3 27.6 65.7 38.9z"/>
      <path class="st47" d="M558.1 315.6l-48.4 27.8 5 2.8 43.4-24.8z"/>
      <path class="st47" d="M623.7 354.6L558 315.7v5.9l60.7 35.9z"/>
      <path class="st54 st55" d="M623.6 354.7l-65.5-39.1-4.2 8.2 61.6 35.6z"/>
      <path class="st46" d="M613.4 283.3L565.1 311l65.7 38.9 48.2-27.7z"/>
      <path class="st47" d="M613.5 283.1L565.1 311l5 2.8 43.4-24.9z"/>
      <path class="st47" d="M679.1 322.2l-65.7-38.9v5.9l60.6 35.9z"/>
      <path class="st54 st55" d="M678.9 322.2l-65.4-39.1-4.2 8.2 61.6 35.7z"/>
      <g id="passanger-3">
        <path class="st54 st67" d="M731.3 429.4s.8-.1.4-.5c-.1-.1-.8-.3-1.3-.4h-1.1s-.7-.1-1.6 0c-1 .2-1.6.5-1.2.7.1.1.6.1.8.2.2.1 1 .2 1 .2l.1-.1c.3.1.6.1.9.2h.1-.3l-.9.2-.4.1-.3.1-.3.2c0 .1.9.5.9.5s.7.5 1 .6c.4.2 1.7.6 1.7.6l.8.2.4.1h.1l.4.1.6.1.3.2 1.3.9.6.5v.2l.5.8-.1.2.3.3h-.1l.1.1h.1c-.1.1-.3.2-.7.3-.2 0 .1.3 1.5.2.3 0 .6-.1.8-.2.4-.1 1.6-.1 1.7-.2l-.2-.1-.4-.1h.1l-.4-.1.2-.5-.4-.5-.4-.5v-.2l-.3-.4-.9-.8h.4l2.6.8.7.5.4.1 1.9 1 .6.1c.2.1.5.2.6.2.1 0 .1.1.3.1.3 0 .9 0 1.1-.1.3 0 .8-.1.9-.2 0-.1-.4-.1-.6-.2-.1 0-.3-.2-.3-.2l.1-.3-1.2-.5-.9-.5-.6-.2-1.3-.7-1-.4-.6-.3c.2-.1.3-.2.5-.2h.4c.1 0 .1-.1.1-.1-.1-.1-.4-.2-.7-.3l-1.8-.5c.2-.1.6-.2.7-.2.1-.1-.2-.3-.2-.3l-.8-.3s-1.5-.4-2-.5c-.6-.1-1.4-.1-1.4-.1h-3.3c-.1.2 0 .2 0 .1z"/>
        <path class="st68" d="M736.7 436.6c.1.2.7.3 1 .3.3 0 .9 0 1-.2.1-.1 0-.5 0-.6 0-.3.1-1.3.1-1.3l-1.2-.4-.7.7s.1.6 0 .8c0 .1-.3.5-.2.7zm8.5-.3c.2 0 .7.3 1 .3 1.4 0 2.1-.4 2.1-.4s-.1-.4-.2-.5c-.2-.2-.7-.2-.9-.3-.7-.3-1.2-1-1.2-1l-2.3.6-.2.7s-.1.3 0 .4c.2.4 1.3.2 1.7.2z"/>
        <path class="st69" d="M736.7 431.8l-.2 2.3.5.9s.9-.4 1.2-.4c.2 0 .8.2.8.2l.4-.5v-4.5l.2-.6-.2-2.1 1-3.9h.4l.6 3.5.3 1.5.3.7.5 2.1.4 2 .9 1.7-.2.5s1.2.3 1.5.2c.3-.1 1.1-.8 1.1-.8l-.1-.5h-.1l-.2-1.3-.4-.8-.9-3.2-.2-.7-.3-2-.4-3.9-.2-1.7-2.2-.2-3.1-1.3-1.2 2.3v2l-.2 1.9.1 3.3-.1 1.1v2.2z"/>
        <path class="st70" d="M738.8 419.3l-1 .6-.7 5.1.4 2.6.6.1.5-.8 1.2-3.8-.8-1 .9.5h.8l1.1-.1-.7.4 1.4 5.4.5.2.5-.3-.3-5.1-.2-1.8-.3-.2-.5-.9-1.1-.3-.4 1.8-.5-.1.3-1.9z"/>
        <path class="st71" d="M744.1 420.1l-1.1-.4.5 1.8.3-.6zm-1.8-10.4l-.4-.1-.1-1.1-1.8.1v.8l-.6.2-.1 2 2.9.7.3-1.6z"/>
        <path class="st71" d="M742.7 407.1c0-1.2-.8-1.7-1.7-1.7-.9 0-1.7.5-1.7 1.7s.8 2.8 1.7 2.8c.9 0 1.7-1.5 1.7-2.8z"/>
        <path class="st72" d="M744.9 411.3c-.1-.3-.6-.8-.6-.8l-.9 2.2-.4 7.1 1.1.6.2-.4.3-1.1s.5-2 .5-2.7c0-.6-.1-2.6-.1-2.6s.1-1.8-.1-2.3z"/>
        <path class="st73" d="M737.1 419.3s2.2.9 3.7 1.1c.5.1 2.4.1 2.4.1l.1-1s.3-.6.3-.8c.2-1.2-.1-3.6.1-4.8.1-.4.4-1.1.4-1.4.1-.5.1-2 .1-2l-2.2-.8s.2 1.8-.8 1.9c-1.5.2-1.9-1.9-1.9-1.9-1.8.4-2.2.9-2.2.9s.7 1.4.8 2c.1.7-.5 2.7-.5 2.7l-.3 4z"/>
        <path class="st74" d="M742.1 417.3c.9-1.2 1.1-4.3 1.3-5.7v-1.4l-1.1-.4s0 1.1-.1 1.6c-.1 1.3-.1 3.9-.7 5-.4.7-2.6 2.1-2.6 2.1l.1 1s2.6-1.6 3.1-2.2z"/>
        <path class="st75" d="M737.7 417l-1.2.2-.8 2.8.6.7 2.6-2.5z"/>
        <path class="st71" d="M741.7 418.2c.1 0 .2-.2.2-.2s.2-.1.2-.2.1-.3.1-.3l.1-.1c0-.1.1-.3.1-.3l.2-.2c0-.1-.2-.4-.2-.4l-.8-.2-.1-.2h-.2c-.2.1-.4.3-.6.4h-.5l-.2 1.2.4.1s.5.4.7.4c.2.1.5.1.6 0z"/>
        <path class="st76" d="M742.6 408.8s.4-1 .4-1.3c.1-.3.4-.8.3-1.1-.1-1.1-1.1-2.1-2.2-2.2-1-.2-1.4.5-1.4.5s-.7.4-.8.6c-.3.4-.6 1.3-.5 1.8.2 1.3 1.1 1.5 1.1 1.5s-.3-1.5-.1-1.4c.2.1.5.1.5.1s-.4-1.2-.2-1c.4.3 1.5.7 1.5.7l-.1-.9s1 .6 1.3 1.2c.1.3 0 .8 0 1.1 0 .2.2.4.2.4z"/>
        <path class="st72" d="M738.1 412.6c-.1-1.6-.9-2-.9-2s-.6.4-1 1.1c-.3.6-.8 2.8-.8 2.8l-.2 1.4s0 .8.2 1c.2.2.8.6 1.1.6.3.1.8.2 1 .3.6.1 2.5 0 2.5 0l.3-1.2-2.9-.8c0-.2.3-1.2.3-1.2s.5-1 .4-2z"/>
        <path class="st77" d="M741.8 409.6s-.7.8-1.4.1c-.1-.1.1 1 .8.9.6-.1.6-1 .6-1z"/>
        <path class="st70" d="M746 433.9l-1.2.5-.8.2.8.1 1.3-.6zm-8.3-.5l-1 .7.9-.3 1.5.5z"/>
        <path class="st78" d="M741.2 411.2c-1.1.2-1.5-1.7-1.5-1.7l-.3.1s.4 2.1 1.9 2c1.1-.1.8-1.9.8-1.9l-.2-.1s.2 1.5-.7 1.6zm2 9.3v-1s-1.9 0-2.5-.1c-.5-.1-1.9-.5-1.9-.5l-.3 1s.7.3 2.1.6c.7.1 2.6 0 2.6 0z"/>
        <path class="st74" d="M735.9 421.8c.1 0 .2-.2.3-.2.3 0 .6.6.9.5.9-.1 2.3-2.9 2.3-2.9s.3-.9-.5-1c-.9-.1-2.6 1.1-3.1 1.8-.2.3-.2 1-.2 1.3 0 .1.1.5.3.5z"/>
        <path class="st78" d="M738 414.5c.4-.4.6-1.3.5-2.3-.2-1.7-.9-1.8-.9-1.8l-.3.3s.6.3.8 1.5c.2 1.3-.3 2.5-.3 2.5s.1-.2.2-.2zm5.8-.6s.3-.9.4-1.3c.1-.5.1-2.1.1-2.1l-.4-.2v1.6c-.1.6-.1 2-.1 2z"/>
      </g>
      <g id="passanger-2">
        <path class="st54 st67" d="M715.3 432.5c-.1 0-.4 0-.7-.1-.1-.1-.3-.2-.5-.3-.4-.2-1.4-.7-2.3-.9-.4-.1-1.7-.3-2.7-.3-1.6 0-2.4 0-2.9.2-.9.2.1 1 1 1.3.1 0 .3.1.4.1-.2.1.1.4.2.5l.1.1s.6.7 1.6.9c.2 0 .8.1 1.2.1l.1.1-.5.4 1.1.1c.3.2.6.4.8.6.3.2 2.5 1.2 2.5 1.2h.6l.7.4s3 1.3 3.5 1.7c.1.1.8.8 1.1.7.6 0 .9-.1 1-.2.1-.1.1-.4.1-.4l.2.1.2-.1-.2-.1-.2-.2c-.2-.1-.8-.1-.8-.1-.2-.1-.4-.1-.5-.2-.5-.3-.5-.8-.9-1-.1-.1-.9-.4-.9-.4l-.3-.2h.6l.5.3s3 1.3 3.5 1.7c.1.1.2.4.2.4s-.3.5-.1.5c.2.1.6-.2.9-.2.6 0 1.1-.6 1.1-.6s.2-.2.1-.3c-.2-.1-.9-.1-.9-.1-.2-.1-.4-.1-.5-.2-.5-.3-.5-.8-.9-1-.1-.1-.9-.4-.9-.4l-.4-.3h.1s-.6-.4-.7-.6c-.1-.1-.5-.5-.7-.6 0 0-.1 0-.1-.1l.7-.9h-.3l-1.6-.1c.2-.1.4-.2.4-.3-.1-.2-1.7-.7-1.7-.7h.2c0 .1-1.7-.4-2.5-.5zm-5.3 1.3l-.5-.5-.6-.1.6.1.3.1.6.4h-.4zm7.7 0s-.2.1-.5.2l-.7-.1-.1-.1-.9-.7.5.1h.1l1.6.6zm-8.8-.6l.6.1z"/>
        <path class="st79" d="M720.5 408.6h3.8v4.3h-3.8z"/>
        <path class="st72" d="M723 438.4l.1-1 .5 1.5c.1.2.5.6.9.7.2 0 .6 0 .7-.2.1-.2-.5-1.1-.5-1.1l-1.6-2.6s-.4 0-.4.5c0 .2.1.8.1.8l.1 1.4h.1zm-2.3 0l.1-1 .5 1.5c.1.2.5.6.9.7.2 0 .6 0 .7-.2.1-.2-.5-1.1-.5-1.1l-1.6-2.6s-.4.1-.4.6c0 .2.1.7.1.7l.1 1.4h.1z"/>
        <path class="st80" d="M722.5 431.1c.1 1 .7 3 .7 4 0 .4-.3 1.1-.2 1.5.1.5.6 1.5 1 1.8.3.2.7 0 .7 0s-.3-1.3-.4-1.7c-.2-1.7.2-6.9.2-6.9v-2.3l-2 .4.2 1.7c0 .1-.2 1.2-.2 1.5zm-2.3 0c.1 1 .7 3 .7 4 0 .4-.3 1.1-.2 1.5.1.5.6 1.5 1 1.8.3.2.7 0 .7 0s-.3-1.3-.4-1.7c-.2-1.7.2-6.9.2-6.9v-2.3l-2 .3.2 1.8c0 .1-.2 1.2-.2 1.5z"/>
        <path class="st77" d="M721.5 410.5h1.7v3.8h-1.7z"/>
        <path class="st73" d="M722 428.8c1.8 0 2.9-.6 2.9-.6s.2-4 .2-4.7c0-1.1-.4-4.3-.4-4.3h-4.1s-1 3.2-1 4.5c0 .5.2 2 .3 2.5.1.6.2 2.3.2 2.3s.7.3 1.9.3z"/>
        <path class="st78" d="M720.6 419.2s-1 3.2-1 4.5c0 .5.2 2 .3 2.5.1.6.2 2.3.2 2.3s.3.1 1 .2c0-.5-.1-1.7-.2-2.1-.1-.6-.3-2.1-.3-2.7 0-1.3 1-4.7 1-4.7h-1z"/>
        <path class="st72" d="M725.4 415.1s-.2-1.8-.5-2.2c-.3-.4-1.7-1-1.7-1l-.2 2.1-1.4-2.1s-1.7.5-2 .9c-.4.5-.9 2.7-.9 2.7l1.5.7.2-.5.3 4h4.2l-.2-3.2.3-.8.4-.6z"/>
        <path class="st69" d="M723.5 416.9l-5.4 2.8 2 4.1 5.5-2.9z"/>
        <path class="st71" d="M723.9 409.1c0-1.2-.7-1.7-1.5-1.7s-1.5.6-1.5 1.7.7 2.4 1.5 2.4c.8.1 1.5-1.2 1.5-2.4z"/>
        <path class="st81" d="M725 412.4c.3-1.1-.1-4.3-1-5.2-.5-.5-1.1-.8-2.2-.6-.7.1-1.4.7-1.5 1.1-.4.8-.5 2.6-.5 3.4 0 .7 0 1.8.7 2.7.4.5 1.2.5 1.2.5s-.6-.7-.6-.9c-.2-.9 0-3.6 0-3.6s.8-.5 1.2-1.2c.2-.4.3-.7.4-.9.1.3.3.7.4.9.3.6.7.9.7.9s.2 1.4.2 1.8c.1 1.5-.3 2.3-.3 2.3 1 .1 1.2-.7 1.3-1.2z"/>
        <path class="st71" d="M723.9 417.9h-.4l-.4.2-.3.3s0 .1.1.1.2-.1.2-.1l.3-.2.2-.1-.2.1-.3.2-.2.2s0 .1.1.1.2-.1.2-.1l.3-.2.2-.1-.2.1-.3.2-.2.2s0 .1.2.1c.1 0 .2-.2.2-.2l.3-.2h.1v.1l-.2.1-.2.2-.1.2s.1.1.2 0c.1 0 .2-.2.2-.2h.3l.4.1s.9-.3 1-.6c.4-.7 0-3.4 0-3.4l-.6.4-.2.6.2 1.8-.5.2-.4-.1zm-5.1-2.4s-.5 1.9-.3 2.6c.3 1 2.6 3.5 2.6 3.5l.3.8s.3.7.6.7c0 0 .1-.1.2-.1 0 0-.1-.1 0-.2 0 0 .1.1.2.1 0 0 .1 0 .2-.1 0 0-.1-.2 0-.2l.1.1c.1 0 .2 0 .2-.1 0 0-.1-.1-.1-.2l.1.1s.1 0 .2-.1c.1-.2-.4-.8-.4-.8h.2c.2 0 .4.1.5 0v-.1s-.3-.2-.4-.2c-.3-.1-.9-.1-1.1-.3-1.5-2.7-2.1-3.3-2.1-3.3l.5-1.7-1.5-.5z"/>
        <path class="st11" d="M723.2 411.5l-.3 2.4-1.4-2.4-.4.5.1 1.1h.5l-.2.5 1.5.8.7-1.3-.2-.2.3-.7zm-4.5 3.5l-.1.4 1.5.7.1-.4zm6.7-.2l-.6.3.1.4.5-.4z"/>
        <path class="st82" d="M724.5 414.2l.3.9.2-.1zm-.6 2.1c.4-.2.4-.6.4-.6s-2.3.3-3-.1c-.3-.2-.8-1.2-.8-1.2l-.6 1.3.3.1.1-.1.2 2.8.5-.3s-.1-1.5.2-1.7c.4-.3 2.1 0 2.7-.2z"/>
        <path class="st70" d="M718.1 419.7l-.1.2 1.8 3.9h.3z"/>
      </g>
      <g id="passanger-1">
        <path class="st54 st67" d="M585.5 555.9c-.8.3-.6 1.1-.1 1.4.3.2 1.5.6 2.2.8.1 0 .2.1.4.1h-.3l1.7.3 1.8-.2-1.6.2 1.5.3v.1s2.3 1.4 2.9 1.9c.3.3 1.1 1.1 1.2 1.1.1 0 .9.2.9.2l-.5.1c0 .1 1 .2 1 .2h.2v.3s-.1.2.2.2c.4.1 1.6.1 2 .1.5 0 .9-.2.9-.3 0-.1-.3-.2-.5-.3h.1s.4-.1.3-.2c-.1 0-.8-.1-.9-.2-.1 0 .3-.1.3-.2.1-.2-1-.8-1.3-1-.5-.5-1.4-1.8-1.4-1.8h2.3s2.8 1 3.6 1.4c.8.4 1.5 1.1 3 1.5.1 0 .6.1.8.1.2.1-.2.2-.1.3.1 0 .6.1.9.2.1.1-.3-1.8-.6-1.9-1-.5-3.3-1.8-3.3-1.8l.2-.2h.4l.2-.4h-.4c-.2-.2-.5-.5-.7-.6-.2-.1-.8-.3-1.1-.4-.8-.3-1.5-.9-2.9-1.2-.9-.2-4.3-.4-4.3-.4l-.9-.2-.3-.2c.3-.1.5-.2.5-.2s0-.1-.1-.1c.3 0 .4-.1.4-.1-.1-.1-.4-.2-.6-.2h-.1c0-.1-.1-.2-.4-.3-.3-.2-1.3-.5-3.4-.5-2.5 0-3.3.1-2.9.4.2.2.7.3 1.1.4-.2 0-.2.1 0 .2s.6.1.8.1c.1 0 .2.1.3.1.2 0 .5.1.9.2l.2.1-.7.1c-.9.2-3.4.3-3.8.5zm14.3 1.7l1.1.6.2.2-.4-.1-.7-.2-.3-.2s-1.2-.5-1.5-.7c-.1-.1-.3-.2-.3-.2l1.9.6zm-9.4 0c.3.1.7.6.7.6v.2l-1.5-.3c-.3-.1-1.1-.5-1.2-.6-.1-.2.1-.6.1-.6s1.5.5 1.9.7z"/>
        <path class="st83" d="M599.6 562.1c.3-.1.5-.7.6-1 .1-.2 0-1 0-1h-1.9s-.4 1.2-.5 1.6c0 .1-.1.4 0 .4.3.3 1.4.2 1.8 0zm6.8.2c.3.1 1.1 0 1.3-.2.1-.1-.1-.6-.1-.7-.1-.4-.5-1.5-.5-1.5h-1.7s-.1 1 0 1.4c.1.3.7.9 1 1z"/>
        <path class="st84" d="M598 554.7c-.1 1-.3 3.1 0 4 .1.2.5.4.5.6 0 .2-.5.3-.5.5 0 .1.2.5.2.5l1.9.2s.5-.6.5-.9c0-.3-.5-.8-.4-1.1 0-.1.3-.3.4-.4.6-1.3.1-4.4.2-5.8.1-1.4.8-5.5.8-5.5h1.6s1.1 5.4 1.4 7.3c.1 1 0 3.1.4 4 .1.2.4.4.4.6 0 .2-.4.4-.4.6 0 .2.4.6.4.6l2 .1s.4-.7.4-.9c0-.2-.4-.2-.5-.4-.1-.2.3-.8.3-.9 0-.1-.5-3.3-.6-4.4-.2-2-.5-7.7-.5-7.7l-1-3h-6.2l-1.1 2.7s.1 5.3 0 7.2c-.1.7-.2 1.6-.2 2.1z"/>
        <path class="st83" d="M605.5 542.9h-6.2l-.2.7s2.1.6 3.5.6 3.2-.6 3.2-.6l-.3-.7z"/>
        <path class="st80" d="M602.8 531.5l-2.3.1v.9l1.2.5 1.2-.8z"/>
        <path class="st77" d="M602.8 531.5s-1.1.9-2.2.1c-.2-.1.1 1.3 1.3 1.2.9-.1.9-1.3.9-1.3z"/>
        <path class="st71" d="M601.1 532.2c.3.1.9.1 1.1 0 .4-.2 1-.8 1.1-1.2.2-.7.2-3 .2-3H600s-.2 2.3 0 3c0 .4.7 1.1 1.1 1.2z"/>
        <path class="st85" d="M603.8 527.7c-.1-1.1-.7-1.5-2.5-1.5-1.5 0-1.8 1.1-1.8 1.8 0 .8.3 1.7.3 1.7s0-1.2.4-1.4c.3-.1 1.1-.2 1.5-.2.3 0 1.3-.1 1.6 0 .3.2.3 1.6.3 1.6s.3-.8.2-2z"/>
        <ellipse transform="rotate(-9.7 599.735 529.944)" class="st71" cx="599.7" cy="530" rx=".3" ry=".6"/>
        <ellipse transform="rotate(-80.305 603.454 530.023)" class="st71" cx="603.4" cy="530" rx=".6" ry=".3"/>
        <path class="st86" d="M596.9 541c0 .8.4 3 .4 3l.5.7.7-.4c-.1-.3-.3-1.5-.3-1.9 0-.8.6-3 .6-3.8.1-.8-.4-2.4-.2-2.6.4-.3 1.1 1.1 1.2 1.6.3.9 0 2.9 0 3.9v1.5c.5.2 1.4.4 2.4.5 1.4.1 2.4-.2 2.9-.4 0 0-.2-1.9-.2-2.6 0-.7 0-2.2.2-2.9.1-.6.4-2.2.7-2.2.4 0 .4 1.7.5 2.2.2.5.7 1.3.8 1.8.1.8-.2 3.2-.2 3.2l-.6 1.3 1 .5s.6-1.2.7-1.7c.2-.8.6-2.4.5-3.2-.1-1.4-1-4.6-1.9-5.7-.6-.7-3-1.1-3-1.1l-3.4.4s-2.2.8-2.6 1.4c-.6 1-.3 3.6-.5 4.7-.1.6-.2 1.4-.2 1.8z"/>
        <path class="st87" d="M598.4 544.3l.3-.2v-3.3l.5-2.4s.1.7.1.9c0 .7-.2 2.6-.2 2.6l.1 1s.2.1.4.1v-1.5c0-1 .3-3 0-3.9-.2-.5-.8-1.9-1.2-1.6-.2.2.3 1.7.2 2.6 0 .8-.6 3-.6 3.8.1.4.4 1.6.4 1.9zm7.5-.5l.3.2.6-1.3s.4-2.4.2-3.2c-.1-.5-.6-1.3-.8-1.8-.2-.5-.1-2.2-.5-2.2-.3 0-.6 1.6-.7 2.2-.1.7-.2 2.2-.2 2.9 0 .6.2 2.6.2 2.6.3-.1.4-.2.4-.2s-.2-1.6-.2-2.2c0-.8.4-3.1.4-3.1s.7 1.6.8 2.2c.1.7 0 2.7 0 2.7l-.5 1.2z"/>
        <path class="st11" d="M598.7 543l-1.8.5.6 1.5 1.4-.9zm7.6-.6l-.6 1.4 1.5.9.8-1.5zm-3.2-8.4l.5-1.2-.7-.6-1.2.8-1.2-.5-.4.7.7 1.2.9-1.1z"/>
        <path class="st88" d="M601 542.1l.9.8 1.1-1-.4-5.8-.6-1.9.4-.5-.7-.4-.5.7.3.4-.5 1.8z"/>
        <path class="st80" d="M605.2 544.6l1.1 1.2.7-1.2-1.3-.8-.6.3-.8.5s.2.3.3.3c.2 0 .6-.3.6-.3zm-5.6.3c.1 0 .1-.3.1-.3l-.8-.5-1.1.8.4.8.7-1s.5.3.7.2z"/>
        <path class="st84" d="M600.4 543.2l-.1.8.4.1v-.8zm3.5.1l-.3.1.1.8.4-.1c.2 0-.2-.8-.2-.8z"/>
      </g>
    </g>
    <g id="round-tree-2">
      <path class="st16" d="M421.6 557.9c-.1.3-.7.7-1.2.8h-.2c-.2 0-.4 0-.6-.1l-8.8-5.2c-.2.6-.6 1.1-1.4 1.5-1.9 1.2-5.1 1.2-7.1 0-1.8-1.1-1.9-2.8-.4-3.9-.5-.1-.9-.3-1.3-.5-2-1.2-2-3 0-4.2 1.9-1.2 5.1-1.2 7 0 .4.2.7.5.9.8 1.9-.9 4.8-.9 6.6.2 1.4.9 1.8 2.1 1.2 3.1.3.1.6.2.8.3.8.5.8 1.3 0 1.8-.2.1-.5.2-.7.3v1.8l5 3c.2-.1.3.1.2.3zm-8.9-5.7l2.2 1.3v-.8c-.2-.1-.5-.2-.7-.3-.2-.1-.3-.3-.5-.4-.3.1-.7.2-1 .2z"/>
      <path class="st17" d="M421.5 557.2c.7.4.8 1.1 0 1.6-.7.4-1.8.4-2.5.1-.1 0-.1-.1-.2-.1s-.1-.1-.2-.1c-.6-.4-.5-1.1.1-1.5.8-.4 2-.4 2.8 0z"/>
      <path class="st18" d="M426.7 529.1c.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9-3.8 0-6.9 3.1-6.9 6.9 0 .7.1 1.4.3 2.1-3.4.4-6.1 3.3-6.1 6.8 0 3.8 3.1 6.9 6.9 6.9 2.4 0 4.5-1.2 5.7-3.1 1.2 1.9 3.3 3.1 5.7 3.1 3.8 0 6.9-3.1 6.9-6.9.1-3.5-2.5-6.4-5.9-6.8z"/>
      <path class="st19" d="M425.9 542.8c3.8 0 6.9-3.1 6.9-6.9 0-3.5-2.7-6.4-6.1-6.8.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9v19.6c1.2 1.9 3.4 3.1 5.8 3.1z"/>
      <path class="st17" d="M418.2 523.8h3.8V558h-3.8z"/>
      <path class="st18" d="M426.7 516c.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9-3.8 0-6.9 3.1-6.9 6.9 0 .7.1 1.4.3 2.1-3.4.4-6.1 3.3-6.1 6.8 0 3.8 3.1 6.9 6.9 6.9 2.4 0 4.5-1.2 5.7-3.1 1.2 1.9 3.3 3.1 5.7 3.1 3.8 0 6.9-3.1 6.9-6.9.1-3.5-2.5-6.4-5.9-6.8z"/>
      <path class="st19" d="M425.9 529.7c3.8 0 6.9-3.1 6.9-6.9 0-3.5-2.7-6.4-6.1-6.8.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9v19.6c1.2 1.8 3.4 3.1 5.8 3.1z"/>
      <circle class="st18" cx="426.1" cy="530.3" r="2.9"/>
      <path class="st17" d="M420.1 537.4c-.3 0-.6-.1-.8-.3-.4-.4-.4-1.1 0-1.6l5.9-5.9c.4-.4 1.1-.4 1.6 0 .4.4.4 1.1 0 1.6l-5.9 5.9c-.2.2-.5.3-.8.3z"/>
      <circle class="st18" cx="425.6" cy="541.2" r="2.3"/>
      <path class="st17" d="M420.9 546.7c-.2 0-.4-.1-.6-.3-.3-.3-.3-.9 0-1.2l4.6-4.6c.3-.3.9-.3 1.2 0 .3.3.3.9 0 1.2l-4.6 4.6c-.2.3-.4.3-.6.3z"/>
      <circle class="st19" cx="413.1" cy="535.4" r="3.4"/>
      <path class="st17" d="M420 543.6c.3 0 .7-.1.9-.4.5-.5.5-1.3 0-1.8l-6.7-6.7c-.5-.5-1.3-.5-1.8 0s-.5 1.3 0 1.8l6.7 6.7c.3.2.6.4.9.4z"/>
    </g>
    <g id="round-tree-1">
      <path class="st16" d="M461.3 580.1c-.1.3-.7.7-1.2.8h-.2c-.2 0-.4 0-.6-.1l-8.8-5.2c-.2.6-.6 1.1-1.4 1.5-1.9 1.2-5.1 1.2-7.1 0-1.8-1.1-1.9-2.8-.4-3.9-.5-.1-.9-.3-1.3-.5-2-1.2-2-3 0-4.2 1.9-1.2 5.1-1.2 7 0 .4.2.7.5.9.8 1.9-.9 4.8-.9 6.6.2 1.4.9 1.8 2.1 1.2 3.1.3.1.6.2.8.3.8.5.8 1.3 0 1.8-.2.1-.5.2-.7.3v1.8l5 3c.3-.1.3.1.2.3zm-8.9-5.7l2.2 1.3v-.8c-.2-.1-.5-.2-.7-.3-.2-.1-.3-.3-.5-.4-.3.1-.6.2-1 .2z"/>
      <path class="st17" d="M461.2 579.4c.7.4.8 1.1 0 1.6-.7.4-1.8.4-2.5.1-.1 0-.1-.1-.2-.1s-.1-.1-.2-.1c-.6-.4-.5-1.1.1-1.5.9-.5 2.1-.5 2.8 0z"/>
      <path class="st18" d="M466.4 551.3c.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9-3.8 0-6.9 3.1-6.9 6.9 0 .7.1 1.4.3 2.1-3.4.4-6.1 3.3-6.1 6.8 0 3.8 3.1 6.9 6.9 6.9 2.4 0 4.5-1.2 5.7-3.1 1.2 1.9 3.3 3.1 5.7 3.1 3.8 0 6.9-3.1 6.9-6.9.2-3.5-2.5-6.4-5.9-6.8z"/>
      <path class="st19" d="M465.6 565c3.8 0 6.9-3.1 6.9-6.9 0-3.5-2.7-6.4-6.1-6.8.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9v19.6c1.3 1.9 3.4 3.1 5.8 3.1z"/>
      <path class="st17" d="M458 546h3.8v34.2H458z"/>
      <path class="st18" d="M466.4 538.2c.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9-3.8 0-6.9 3.1-6.9 6.9 0 .7.1 1.4.3 2.1-3.4.4-6.1 3.3-6.1 6.8 0 3.8 3.1 6.9 6.9 6.9 2.4 0 4.5-1.2 5.7-3.1 1.2 1.9 3.3 3.1 5.7 3.1 3.8 0 6.9-3.1 6.9-6.9.2-3.5-2.5-6.4-5.9-6.8z"/>
      <path class="st19" d="M465.6 551.9c3.8 0 6.9-3.1 6.9-6.9 0-3.5-2.7-6.4-6.1-6.8.2-.7.3-1.4.3-2.1 0-3.8-3.1-6.9-6.9-6.9v19.6c1.3 1.8 3.4 3.1 5.8 3.1z"/>
      <circle class="st18" cx="465.9" cy="552.5" r="2.9"/>
      <path class="st17" d="M459.9 559.6c-.3 0-.6-.1-.8-.3-.4-.4-.4-1.1 0-1.6l5.9-5.9c.4-.4 1.1-.4 1.6 0 .4.4.4 1.1 0 1.6l-5.9 5.9c-.3.2-.6.3-.8.3z"/>
      <circle class="st18" cx="465.3" cy="563.4" r="2.3"/>
      <path class="st17" d="M460.6 568.9c-.2 0-.4-.1-.6-.3-.3-.3-.3-.9 0-1.2l4.6-4.6c.3-.3.9-.3 1.2 0 .3.3.3.9 0 1.2l-4.6 4.6c-.1.2-.4.3-.6.3z"/>
      <circle class="st19" cx="452.9" cy="557.6" r="3.4"/>
      <path class="st17" d="M459.8 565.8c.3 0 .7-.1.9-.4.5-.5.5-1.3 0-1.8l-6.7-6.7c-.5-.5-1.3-.5-1.8 0s-.5 1.3 0 1.8l6.7 6.7c.2.2.6.4.9.4z"/>
    </g>
    <g id="our-goals">
      <text transform="translate(967.95 704.295)" class="st89 st90 st91">
        Our Goals
      </text>
      <text transform="translate(967.95 742.773)">
        <tspan x="0" y="0" class="st92 st93 st94">Our goal is to provide a reliable transportation service that will enhance the </tspan><tspan x="0" y="24.5" class="st92 st93 st94">university town gown and aims to reduce carbon emissions, improve safety, provide </tspan><tspan x="0" y="49" class="st92 st93 st94">customized services for the physically disabled and modernize the campus lifestyle.</tspan>
      </text>
      <g id="goals-icon-1">
        <path class="st95" d="M1050 885.2c-2.4 0-4.3 1.9-4.3 4.3s4.3 10.2 4.3 10.2 4.3-7.8 4.3-10.2c0-2.4-1.9-4.3-4.3-4.3zm0 6c-1.2 0-2.1-.9-2.1-2.1 0-1.2.9-2.1 2.1-2.1 1.2 0 2.1.9 2.1 2.1 0 1.2-.9 2.1-2.1 2.1z"/>
        <path class="st96" d="M1050 932.7h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-1.9h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-1.9h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-1.9h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-2h-.5v-1h.5v1zm0-1.9h-.5v-1h.5v1z"/>
        <path class="st95" d="M1098.5 867.4l-6.1 3.5-6.4-7.4 5.5-3.2z"/>
        <path class="st97" d="M1103.7 863.2l-16.3 9.4 3.8 6.6 16.3-9.4c.6-.3.2-2.1-.8-3.9-1-1.9-2.4-3.1-3-2.7z"/>
        <ellipse transform="rotate(-29.99 1089.63 875.866)" class="st98" cx="1089.5" cy="875.8" rx="1.3" ry="3.8"/>
        <path class="st97" d="M1089.8 876.3l-6.7 3.9c-.3.2-.6.1-.8-.2-.2-.3-.1-.6.2-.8l6.7-3.9c.3-.2.6-.1.8.2.1.3 0 .7-.2.8z"/>
        <path class="st99" d="M1080.67 880.674l2.6-1.5.3.52-2.6 1.5z"/>
        <ellipse transform="rotate(-30.003 1081.022 880.703)" class="st100" cx="1081.1" cy="880.7" rx="1.8" ry="1.8"/>
        <path class="st95" d="M1110.3 880.2l-6.1 3.5-8.5-9.9 5.5-3.2zm-29.2-5.7l5.4 9.3c1.9-1.4 2.3-4.3 1-6.8-1.5-2.4-4.2-3.4-6.4-2.5z"/>
        <path class="st101" d="M1077.1 892.9c-3.4-.6-6.3-2.6-8-5.5-1.7-3-2-6.5-.8-9.7l.6.2c-1.1 3-.8 6.4.8 9.2 1.6 2.8 4.4 4.7 7.6 5.3l-.2.5z"/>
        <path class="st101" d="M1075.8 889.8c-3.7-1.5-6-5.4-5.4-9.4l.6.1c-.5 3.7 1.6 7.4 5.1 8.8l-.3.5z"/>
        <path class="st101" d="M1075.9 887c-1.8-1.1-3-3.1-3-5.2h.6c0 1.9 1.1 3.7 2.7 4.7l-.3.5zm.9-2.5c-.7-.6-1.2-1.4-1.4-2.4l.6-.1c.1.8.5 1.5 1.1 2l-.3.5z"/>
        <path class="st102" d="M1055.2 916.3h25.9v55.2h-25.9z"/>
        <path class="st103" d="M1060.6 920.9h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm-13.4 6.8h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm-13.4 6.8h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm-13.4 6.7h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm-13.4 6.8h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm-13.4 6.8h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm3.4 0h1.6v4.7h-1.6zm3.3 0h1.6v4.7h-1.6zm-13.4 9.1h15v6.4h-15z"/>
        <path class="st104" d="M1078 916.3c-1.4-4.3-5.3-7.4-9.8-7.4-4.6 0-8.5 3.1-9.8 7.4h19.6z"/>
        <path class="st105" d="M1021.2 971.3V924h5.7c.2 0 .4-.2.4-.4v-3.4h13.2v3.4c0 .2.2.4.4.4h5.7v47.3h-25.4z"/>
        <path class="st106" d="M1040.5 923.6v-3.4h-6.6v51.1h12.7V924h-5.7c-.2 0-.4-.2-.4-.4z"/>
        <path class="st107" d="M1024.4 955h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm5 0h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm-15.2-6.3h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm5 0h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm-15.2-6.4h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm5 0h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm-15.2-6.3h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm5 0h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm-15.2-6.4h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm5 0h3.8v4.7h-3.8zm5.1 0h3.8v4.7h-3.8zm-11.2 33h2.4v8.3h-2.4zm4.3 0h2.4v8.3h-2.4zm4.3 0h2.4v8.3h-2.4z"/>
        <path class="st11" d="M1082.9 936.1h7.9V971h-7.9z"/>
        <path class="st108" d="M1091 971.3h-8.3v-35.4h8.3v35.4zm-7.8-.5h7.4v-34.4h-7.4v34.4z"/>
        <path class="st11" d="M1090.8 936.1h-7.9v-3.4l4-6.2 3.9 6.2z"/>
        <path class="st108" d="M1091 936.4h-8.3v-3.8l4.2-6.5 4.2 6.5v3.8zm-7.8-.5h7.4v-3.2l-3.7-5.7-3.7 5.7v3.2z"/>
        <path class="st11" d="M1086.9 926.5l-2 3.1h3.9z"/>
        <path class="st108" d="M1089.3 929.8h-4.8l2.4-3.8 2.4 3.8zm-3.9-.5h3l-1.5-2.3-1.5 2.3zm-.2 10.6h.5v25.9h-.5zm1.4 0h.5v25.9h-.5zm1.4 0h.5v25.9h-.5z"/>
        <path class="st11" d="M992 936.6h7.9v34.9H992z"/>
        <path class="st108" d="M1000.1 971.8h-8.3v-35.4h8.3v35.4zm-7.8-.5h7.4v-34.4h-7.4v34.4z"/>
        <path class="st11" d="M999.9 936.6H992v-3.5l3.9-6.1 4 6.1z"/>
        <path class="st108" d="M1000.1 936.9h-8.3V933l4.2-6.5 4.2 6.5v3.9zm-7.8-.5h7.4v-3.2l-3.7-5.7-3.7 5.7v3.2z"/>
        <path class="st11" d="M995.9 927l-1.9 3.1h3.9z"/>
        <path class="st108" d="M998.4 930.3h-4.8l2.4-3.8 2.4 3.8zm-4-.5h3l-1.5-2.3-1.5 2.3zm-.1 10.6h.5v25.9h-.5zm1.4 0h.5v25.9h-.5zm1.4 0h.5v25.9h-.5z"/>
        <path class="st105" d="M997.2 942.5h21.1v28.8h-21.1z"/>
        <path class="st106" d="M1007.7 942.5h10.6v28.8h-10.6z"/>
        <path class="st109" d="M1011.7 946.5h2.8v24.8h-2.8zm-5.4 0h2.8v24.8h-2.8zm-5.3 0h2.8v24.8h-2.8z"/>
        <path class="st102" d="M1000.5 929.1h14.5v13.5h-14.5z"/>
        <path class="st110" d="M1007.7 929.1h7.3v13.5h-7.3z"/>
        <path class="st105" d="M1004.7 922.4h6v6.7h-6z"/>
        <path class="st111" d="M1003.9 922.4l3.6-6.1h.5l3.6 6.1z"/>
        <path class="st112" d="M1006 923.4h.7v4.4h-.7zm1.4 0h.7v4.4h-.7zm1.4 0h.7v4.4h-.7z"/>
        <path class="st113" d="M1004 933.1h2.6v9.4h-2.6zm5 0h2.6v9.4h-2.6z"/>
        <path class="st114" d="M1096.9 972.3H983.5c-.4 0-.7-.4-.7-.9s.3-.9.7-.9h113.4c.4 0 .7.4.7.9 0 .6-.3.9-.7.9z"/>
        <path class="st115" d="M1062.9 978.7c0 .9-.8 1.7-1.7 1.7h-22.3c-1 0-1.7-.8-1.7-1.7v-39.6c0-.9.8-1.7 1.7-1.7h22.3c1 0 1.7.8 1.7 1.7v39.6z"/>
        <path class="st116" d="M1039.8 942.3h20.4v32.5h-20.4z"/>
        <path class="st117" d="M1050 976.2c.7 0 1.2.5 1.2 1.2s-.5 1.2-1.2 1.2-1.2-.5-1.2-1.2c0-.6.5-1.2 1.2-1.2zm0-.4c-.9 0-1.6.7-1.6 1.6 0 .9.7 1.6 1.6 1.6.9 0 1.6-.7 1.6-1.6 0-.8-.7-1.6-1.6-1.6z"/>
        <path class="st118" d="M1048.9 957.1l.4-14.8h-9.5v19z"/>
        <path class="st119" d="M1055 939.9c0 .3-.3.6-.6.6h-8.8c-.3 0-.6-.3-.6-.6s.3-.6.6-.6h8.8c.3 0 .6.3.6.6z"/>
        <path class="st120" d="M1048 954v-11.7h-8.2v15.6z"/>
        <path class="st121" d="M1039.8 967.2h10.1v.8h-10.1zm9.2 4.1h11.2v.8H1049z"/>
        <path class="st122" d="M1045.4 956.015l2.275-1.036.456 1-2.27 1.03z"/>
        <path class="st123" d="M1040.22 958.768l2.274-1.036.29.637-2.275 1.03z"/>
        <path class="st122" d="M1044.9 956.3l-.6.3-.1-.3-1.1.5.2.3-.6.2.4 1 2.2-1z"/>
        <path class="st100" d="M1060.2 962.6v-1.2l-10.4-5v-14.1h-1.1v14.1l-8.9 4.3v1.3l8.9-4.4v17.2h1.1v-17.2z"/>
        <path class="st122" d="M1051.2 959.8h1v1.9h-1z"/>
        <path class="st122" d="M1053.7 960.1l-2.5-1.3-.7.5v4.6h1v-3.7l2.2 1.1zm-3.2 4.5h1.2v2.5h-1.2z"/>
        <path class="st122" d="M1050.5 964.6h2.2v1h-2.2z"/>
        <path class="st123" d="M1052.6 969v-1h-2.1v2.9h2.1v-.9h-1v-1zm1.7-.9h4v1.2h-4zm1.2 1.6h4v1.2h-4z"/>
        <path class="st123" d="M1056 968.7h2v1.4h-2z"/>
        <path class="st120" d="M1060.2 963.2l-5.9-3v7.4h5.9z"/>
        <path class="st120" d="M1052.2 962.2h4.1v1.7h-4.1zm1.1 2.4h2.5v3h-2.5z"/>
        <path class="st122" d="M1047 959.8h1v2.9h-1zm0 3.4h1v3.4h-1z"/>
        <path class="st122" d="M1045.8 964.2h1.7v1.4h-1.7z"/>
        <path class="st122" d="M1043.8 964.5h3v.8h-3z"/>
        <path class="st123" d="M1040.58 962.198l5.21-2.548.528 1.078-5.21 2.548zm-.08 2.002h1.3v2.4h-1.3z"/>
        <path class="st122" d="M1050.9 942.3h1.6v6.2h-1.6zm1.9 0h.6v6.2h-.6z"/>
        <path class="st120" d="M1054.7 942.3h.6v6.2h-.6zm0 7h.6v2.8h-.6z"/>
        <path class="st122" d="M1050.9 949.5h1.1v6.1h-1.1z"/>
        <path class="st123" d="M1052.5 950h.8v1.9h-.8zm0 2.3h.8v1.4h-.8z"/>
        <path class="st122" d="M1058.6 956.7h1.1v3.2h-1.1zm-4.832.675l.444-.896 3.046 1.51-.444.89z"/>
        <path class="st120" d="M1056 951.9c0 1.9 1.2 3.5 3 4.1l1.2.3v-13.9h-4.2v9.5z"/>
        <path class="st122" d="M1040.5 968.8h1v5h-1zm1.8.1h5.2v1.2h-5.2z"/>
        <path class="st123" d="M1042.3 970.8h1.7v.8h-1.7zm2 0h.8v.8h-.8zm1.2 0h.8v.8h-.8zm1.1 0h.8v.8h-.8z"/>
        <circle class="st123" cx="1045" cy="963" r=".8"/>
        <path class="st120" d="M1047.5 973.1c0 .5-.4.8-.8.8h-3.5c-.5 0-.8-.4-.8-.8 0-.5.4-.8.8-.8h3.5c.5 0 .8.3.8.8zm3-.5h9.2v.5h-9.2z"/>
        <path class="st122" d="M1050.5 973.5h9.2v.9h-9.2zm5.192-17.282l1.408-1.42 1.42 1.406-1.407 1.42zm-1.012-1.972l1.833-.802.52 1.192-1.832.8zm-3.78.754v1l2.4 1.2.5-.9zm-7.1 9.5h1.1v2.1h-1.1z"/>
        <path class="st95" d="M1051.6 963.7c-.9 0-1.6.7-1.6 1.6 0 .9 1.6 3.2 1.6 3.2s1.6-2.3 1.6-3.2c0-.9-.7-1.6-1.6-1.6zm0 2.2c-.4 0-.8-.3-.8-.8s.3-.8.8-.8c.4 0 .8.3.8.8s-.3.8-.8.8z"/>
        <path class="st124" d="M1045.1 951.8c0 .8-.6 1.4-1.4 1.4-.8 0-1.4-.6-1.4-1.4v-6.4c0-.8.6-1.4 1.4-1.4.8 0 1.4.6 1.4 1.4v6.4z"/>
        <path class="st125" d="M1039.8 942.3h20.4v3.1h-20.4z"/>
        <path class="st11" d="M1059.1 944.5l-.5-.4c0-.1.1-.2.1-.3 0-.4-.3-.7-.7-.7-.4 0-.7.3-.7.7 0 .4.3.7.7.7.2 0 .3-.1.4-.1l.5.4h.1c.1 0 .1 0 .1-.1.1-.1 0-.2 0-.2zm-1.6-.8c0-.2.2-.4.4-.4s.4.2.4.4-.2.4-.4.4-.4-.2-.4-.4z"/>
        <text transform="translate(984.332 1014.675)">
          <tspan x="0" y="0" class="st92 st90 st94">Modernizing </tspan><tspan x="-14.2" y="24.5" class="st92 st90 st94">College Campus</tspan>
        </text>
      </g>
      <g id="goals-icon-2">
        <path class="st126" d="M1229 922.7s-2.8 3-4.2-4.2c-1.5-7.7-1.4-11.9 1.2-12.7 1.7-.6 2.2.9 2.2.9l.8 16zm5.8 10.8v5.4c0 2 .9 3.9 2.4 5.1l4.7 3.9c2.4 2 5.9 2 8.3 0l4.8-3.9c1.5-1.3 2.4-3.1 2.4-5.1V933l-22.6.5z"/>
        <path class="st127" d="M1234.8 937.5c3.1 3.4 6.9 5.2 11.1 5.2 4.5 0 8.5-2 11.6-5.7v-4l-22.7.5v4z"/>
        <path class="st128" d="M1245.9 940c10.4 0 18.3-10.9 18.3-28.9 0-22.5-6.6-27.7-18.3-27.7-11.8 0-18.3 5.2-18.3 27.7 0 18.1 7.9 28.9 18.3 28.9z"/>
        <path class="st126" d="M1263.1 922.7s2.8 3 4.2-4.2c1.5-7.7 1.4-11.9-1.2-12.7-1.7-.6-2.2.9-2.2.9l-.8 16z"/>
        <path class="st129" d="M1246.2 883.5V940c10.3-.2 18.1-11 18.1-28.9 0-22.3-6.5-27.6-18.1-27.6z"/>
        <path class="st130" d="M1229 946.9l-14.6 9.5c-1.4.9-2.4 2.3-2.8 3.9l-3.2 12.5h37.6V949l-17-2.1z"/>
        <path class="st131" d="M1234.8 938.6h-1.2l-4.6 8.3 11.1 10.9 5.8-8.8z"/>
        <path class="st130" d="M1262.8 946.9l14.6 9.5c1.4.9 2.4 2.3 2.8 3.9l3.2 12.5h-37.6V949l17-2.1z"/>
        <path class="st131" d="M1257 938.6h1.2l4.6 8.3-11 10.9-5.9-8.8z"/>
        <path class="st132" d="M1227.6 911.1s-4.6-2.8-1.5-15.7c2.1-8.5 7.6-8.1 7.6-8.1s-5.5 8.7-6.1 23.8zm36.7 0s4.6-2.8 1.5-15.7c-2.1-8.5-7.6-8.1-7.6-8.1s5.5 8.7 6.1 23.8z"/>
        <path class="st130" d="M1274.3 891.4s-4-6.9-7.4-7.4c-9.5-1.2-16.5-4.6-21.1-4.6-4.5 0-11.5 3.4-21.1 4.6-3.4.4-7.4 7.4-7.4 7.4l7.9 7.8h41.2v.2l7.9-8z"/>
        <path class="st131" d="M1266.5 899.2v.2l7.8-8s-4-6.9-7.4-7.4c-9.5-1.2-16.5-4.6-21.1-4.6v19.8h20.7z"/>
        <path class="st133" d="M1250.9 887.3c-.3 0-.6.2-.6.6h-3.2l-1-3c.2-.1.4-.3.4-.5 0-.3-.2-.6-.6-.6-.3 0-.6.2-.6.6 0 .2.2.4.4.5l-1 3h-2.9c0-.3-.2-.6-.6-.6-.3 0-.6.2-.6.6 0 .3.2.6.6.6.1 0 .2-.1.3-.1l2.4 1.8-1 3h-.1c-.3 0-.6.2-.6.6 0 .3.2.6.6.6.3 0 .6-.2.6-.6 0-.1-.1-.3-.2-.4l2.5-1.8 2.7 1.9c0 .1-.1.2-.1.3 0 .3.2.6.6.6.3 0 .6-.2.6-.6 0-.3-.2-.6-.6-.6-.1 0-.2 0-.3.1l-1-3.1 2.6-1.9c.1.1.3.2.4.2.3 0 .6-.2.6-.6.2-.3 0-.6-.3-.6z"/>
        <path class="st134" d="M1245.9 902.5h20.6l2.1 2.5s-4.6 3.4-22.7 3.4-22.7-3.4-22.7-3.4l2.2-2.5h20.5z"/>
        <path class="st135" d="M1225.4 899.2h41.2v3.3h-41.2z"/>
        <path class="st136" d="M1248.6 893.4c0 .1-.1.2-.1.3 0 .3.2.6.6.6.3 0 .6-.2.6-.6 0-.3-.2-.6-.6-.6-.1 0-.2 0-.3.1l-1-3.1 2.6-1.9c.1.1.3.2.4.2.3 0 .6-.2.6-.6 0-.3-.2-.6-.6-.6-.3 0-.6.2-.6.6h-3.2l-1-3c.2-.1.4-.3.4-.5 0-.3-.2-.6-.6-.6v7.7l2.8 2z"/>
        <text transform="translate(1193.765 1014.675)">
          <tspan x="0" y="0" class="st92 st90 st94">Drastically</tspan><tspan x="-30.2" y="24.5" class="st92 st90 st94">Improving Safety</tspan>
        </text>
      </g>
      <g id="goals-icon-3">
        <path class="st137" d="M1410.5 914.3c.2-3.8 3.7-7.3 7.5-6.3.2-2 3.2-3.2 4.9-2.2.5-9.8 9.8-13.3 15.4-9.1.3-4.6 5.8-6.3 7.6-4 .4-2.2 3.8-2.2 4.9-.6 1.8-4.5 7.5-2.8 7.8-.1 1.9-4.3 11.5-3.4 12.7 2.4 2.1.7.7 3.9-1.2 3.5.5 5.5-5.7 9.9-12.3 6.4 1.4 3.2-2.2 7.6-7 5.5 1.4 1.7.8 4.4-1.9 4.4h-38.4z"/>
        <path class="st11" d="M1446.4 929.5v-9.8l2.4-5.3s-7-1.1-19.1-1.1-19.1 1.1-19.1 1.1l2.4 5.3v9.8l-12.9 43.3h59.2l-12.9-43.3z"/>
        <path class="st138" d="M1412.9 919.6h33.4v9.8h-33.4z"/>
        <path class="st139" d="M1460 949.2h-15.4v-9zm15.3 0H1460v-9zm15.4 0h-15.4v-9z"/>
        <path class="st140" d="M1444.6 949.2h46.1v23.6h-46.1z"/>
        <path class="st11" d="M1448.2 953.6h4.5v9.3h-4.5zm8.9 0h4.5v9.3h-4.5zm8.9 0h4.5v9.3h-4.5zm8.8 0h4.5v9.3h-4.5zm8.9 0h4.5v9.3h-4.5z"/>
        <text transform="translate(1401.605 1014.675)">
          <tspan x="0" y="0" class="st92 st90 st94">Reducing</tspan><tspan x="-41.1" y="24.5" class="st92 st90 st94">Carbon Emissions</tspan>
        </text>
      </g>
      <g id="goals-icon-4">
        <path class="st141" d="M1651 915.2v-10.1l6.4.3 2.5 13.9c0 2.3-1.9 4.1-4.2 4.1H1644v-8.2h7z"/>
        <path class="st11" d="M1641.7 918.8h-1.4c.3-.2.5-.4.7-.6.2.2.4.4.7.6z"/>
        <path class="st142" d="M1637.7 915.8c-1.8 1.8-1.8 4.6 0 6.4 1.8 1.8 4.8 1.8 6.6 0 1.8-1.8 1.8-4.6 0-6.4-1.8-1.7-4.8-1.7-6.6 0z"/>
        <path class="st143" d="M1637.8 920.5c1.8 1.8 4.8 1.8 6.6 0 .6-.5 1-1.2 1.2-1.9.1 1.3-.3 2.6-1.4 3.6-1.8 1.8-4.8 1.8-6.6 0-1.3-1.2-1.7-3-1.2-4.5.2 1 .6 2 1.4 2.8z"/>
        <path class="st10" d="M1644 915.2h5.4v8.2h-5.4z"/>
        <path class="st144" d="M1653.9 916.5l1.1-7v13.8h-11v-3.7h6c2.5 0 3.5-.6 3.9-3.1z"/>
        <path class="st141" d="M1658.1 908.1c1.6-1.6 1.6-4.1 0-5.7-1.6-1.6-4.3-1.6-5.9 0-1.6 1.6-1.6 4.1 0 5.7 1.7 1.6 4.3 1.6 5.9 0z"/>
        <path class="st145" d="M1673.5 968.7h-7.8c0-2.5 3.4-4.7 7.8-5.1v5.1zm-12 0h-11.4c0-2.5 4.9-4.7 11.4-5.1v5.1z"/>
        <path class="st141" d="M1667.2 929H1655v35.8h7.7v-28.6h4.5v28.6h7.7V929z"/>
        <path class="st144" d="M1655 929h19.9v1.4H1655zm15.2 4.1h-11.4v31.7h3.9v-28.6h4.5v28.6h3zm-10.9-31.7h11.3l-.5-.7h-10.2z"/>
        <path class="st141" d="M1655 901.2h19.9v27.7H1655z"/>
        <path class="st11" d="M1656.6 909.5h3.1v1.4h-3.1zm13-8.3l-4.7 10-4.7-10z"/>
        <path class="st146" d="M1660.8 901.8c0 2.2 1.8 3.9 4.1 3.9 2.2 0 4.1-1.8 4.1-3.9v-1.7c0-2.2-1.8-3.9-4.1-3.9-2.2 0-4.1 1.8-4.1 3.9v1.7z"/>
        <path class="st144" d="M1659.4 901.2l-1.2 7.5h2.2l-1.6 2.6 6.2 5.5-4.9-5.6 1.5-3.1-2.7-.1z"/>
        <path class="st144" d="M1670.6 901.2l1.2 7.5h-2.2l1.6 2.6-6.3 5.5 5-5.6-1.6-3.1 2.8-.1z"/>
        <path class="st144" d="M1664.9 916.7h.1V929h-.1z"/>
        <path class="st147" d="M1664.9 911.2l-1.2-2.5.2-.8h2l.1.9zm1-5.6l.5 1.1-.5 1.2h-2l-.6-1.2.6-1.1z"/>
        <path class="st148" d="M1663.8 908.2l.1-.3h2v.3z"/>
        <ellipse class="st142" cx="1665" cy="889.2" rx="12.5" ry="12.1"/>
        <path class="st143" d="M1663.7 898.4c6.9 0 12.5-5.4 12.5-12.1 0-1.2-.2-2.4-.6-3.5 1.2 1.9 1.9 4 1.9 6.4 0 6.7-5.6 12.1-12.5 12.1-5.6 0-10.4-3.6-12-8.5 2.3 3.3 6.2 5.6 10.7 5.6z"/>
        <path class="st149" d="M1677.5 889.2c0 3-1.1 5.7-3 7.8l-3.9-3.6V880h2.6c2.7 2.3 4.3 5.5 4.3 9.2z"/>
        <ellipse class="st149" cx="1655.7" cy="890.8" rx=".9" ry="1.2"/>
        <ellipse class="st149" cx="1663.5" cy="890.8" rx=".9" ry="1.2"/>
        <path class="st149" d="M1665 877.1c5.1 0 9.5 2.9 11.4 7.2l-5.8 5.2c-2.5 0-18.3-4.1-18.3-12.3h12.7z"/>
        <path class="st149" d="M1677.5 889.2c0 .7-.1 1.3-.2 2-1.7-2.5-2.8-6-2.8-9.8 1.9 2.1 3 4.8 3 7.8z"/>
        <path class="st150" d="M1669.1 965.5c1.8 0 3.4 1.4 3.4 3.2h-6.7c-.1-1.8 1.4-3.2 3.3-3.2zm-16 0h1.2l3.4 3.2h-7.5c-.1-1.2 1-2.3 2.9-3.2z"/>
        <ellipse class="st142" cx="1670.7" cy="892.4" rx="3" ry="2.9"/>
        <path class="st151" d="M1627.6 920.2h25.2v2.3h-25.2z"/>
        <path class="st152" d="M1627.6 920.2h25.2v19.1h-25.2z"/>
        <path class="st153" d="M1612.8 968.7c2.5 0 4.5-1.9 4.5-4.3s-2-4.3-4.5-4.3-4.5 1.9-4.5 4.3 2 4.3 4.5 4.3z"/>
        <path class="st154" d="M1611 931.1h25.2v2.3H1611z"/>
        <path class="st155" d="M1613.4 931.1h18.3v3.4h-18.3z"/>
        <path class="st154" d="M1617.4 959.7c.7 0 1.2-.5 1.2-1.1v-11c0-1.9 1.6-3.4 3.5-3.4h8.1c3.9 0 7.1-3.1 7.1-6.8V921c0-1.3 1.1-2.3 2.4-2.3h6.2c.7 0 1.2-.5 1.2-1.1 0-.6-.5-1.1-1.2-1.1h-6.2c-2.6 0-4.7 2-4.7 4.6v16.4c0 2.5-2.1 4.6-4.7 4.6h-8.1c-3.3 0-5.9 2.6-5.9 5.7v11c-.1.4.4.9 1.1.9z"/>
        <path class="st156" d="M1640.8 915.8h8.7v3.2h-8.7z"/>
        <path class="st153" d="M1634.3 968.7c8.9 0 16.2-7 16.2-15.6s-7.3-15.6-16.2-15.6c-8.9 0-16.2 7-16.2 15.6s7.3 15.6 16.2 15.6zm0-28c7.1 0 12.9 5.6 12.9 12.4 0 6.8-5.8 12.4-12.9 12.4-7.1 0-12.9-5.6-12.9-12.4 0-6.8 5.8-12.4 12.9-12.4z"/>
        <path class="st153" d="M1634.3 951.2c1.1 0 2 .9 2 2s-.9 2-2 2-2-.9-2-2c0-1.2.9-2 2-2z"/>
        <path class="st153" d="M1634.5 967.7h-.4v-13.6l-5.7 12.5-.4-.2 5.6-12.4-9.9 9.5-.3-.3 10-9.6-13.2 4.9-.2-.4 13.1-4.9h-14v-.4h14.1l-12.9-5.5.2-.4 12.8 5.4-9.9-9.5.3-.3 10 9.6-5.1-12.7.4-.1 5.1 12.6v-13.5h.4V952l5.7-12.5.4.2-5.6 12.4 9.9-9.5.3.3-10 9.6 13.2-4.9.2.4-13.1 4.9h14v.4h-14.1l12.9 5.5-.2.4-12.8-5.4 9.9 9.5-.3.3-10-9.6 5.1 12.7-.4.1-5.1-12.6v13.5z"/>
        <path class="st153" d="M1633.1 940.8h2.4v12.3h-2.4z"/>
        <ellipse class="st142" cx="1610.4" cy="927" rx="4.7" ry="4.5"/>
        <path class="st143" d="M1610.4 929.8c2.3 0 4.2-1.6 4.6-3.7.1.3.1.6.1.9 0 2.5-2.1 4.5-4.7 4.5s-4.7-2-4.7-4.5c0-.3 0-.6.1-.9.4 2.1 2.3 3.7 4.6 3.7z"/>
        <path class="st143" d="M1610.4 929.8c2.3 0 4.2-1.6 4.6-3.7.1.3.1.6.1.9 0 2.5-2.1 4.5-4.7 4.5s-4.7-2-4.7-4.5c0-.3 0-.6.1-.9.4 2.1 2.3 3.7 4.6 3.7z"/>
        <path class="st10" d="M1631.9 913v.4c-.2 9.7-8.5 17.6-18.7 17.6v-7.9c5.8 0 10.5-4.5 10.5-10.1 0-2.2 1.8-3.9 4.1-3.9s4.1 1.7 4.1 3.9z"/>
        <path class="st157" d="M1631.9 913v.4c-.2 9.7-8.5 17.6-18.7 17.6v-3.7c8.2 0 14.6-6.4 14.6-14.3v-3.9c2.3 0 4.1 1.7 4.1 3.9zm-4.1 18.4h19.4v1.4h-19.4z"/>
        <path class="st10" d="M1627.6 909.1h19.6v22.3h-19.6z"/>
        <path class="st157" d="M1643.3 913c0-2.1 1.8-3.9 4-3.9v15.3c-3.4 4-8.6 6.6-14.4 6.6v-8.8c5.7 0 10.4-3.6 10.4-9.2z"/>
        <path class="st10" d="M1631.9 909.2h11.1l-.6-.6h-9.9z"/>
        <path class="st11" d="M1642 909s-.8 9.7-4.8 9.7c-4.1 0-4.5-9.7-4.5-9.7h9.3z"/>
        <path class="st146" d="M1633.3 909.6c0 2.1 1.8 3.9 4 3.9s4-1.7 4-3.9V908c0-2.1-1.8-3.9-4-3.9s-4 1.7-4 3.9v1.6z"/>
        <path class="st157" d="M1637.3 924.2h.1v7.2h-.1z"/>
        <ellipse class="st142" cx="1637.5" cy="897.2" rx="12.3" ry="11.9"/>
        <path class="st143" d="M1638.8 906.2c-6.8 0-12.3-5.3-12.3-11.9 0-1.2.2-2.4.5-3.5-1.2 1.8-1.9 4-1.9 6.3 0 6.6 5.5 11.9 12.3 11.9 5.5 0 10.2-3.5 11.8-8.4-2.1 3.4-6 5.6-10.4 5.6z"/>
        <path class="st158" d="M1649.9 897.2c0 3-1.1 5.7-3 7.8l-3.9-3.6v-13.3h2.6c2.7 2.2 4.3 5.5 4.3 9.1z"/>
        <ellipse class="st149" cx="1628.3" cy="898.8" rx=".9" ry="1.2"/>
        <ellipse class="st149" cx="1636" cy="898.8" rx=".9" ry="1.2"/>
        <path class="st158" d="M1637.5 885.2c5.1 0 9.5 2.9 11.4 7.1h-14.8c-2.5 0-4.7-1.2-6-3-.9-1.2-1.4-2.6-1.4-4.1h10.8z"/>
        <ellipse class="st142" cx="1643" cy="899.4" rx="2.1" ry="2"/>
        <ellipse class="st142" cx="1630" cy="927" rx="4.7" ry="4.5"/>
        <path class="st143" d="M1630 929.8c2.3 0 4.2-1.6 4.6-3.7.1.3.1.6.1.9 0 2.5-2.1 4.5-4.7 4.5s-4.7-2-4.7-4.5c0-.3 0-.6.1-.9.4 2.1 2.3 3.7 4.6 3.7z"/>
        <path class="st10" d="M1651.4 913v.4c-.2 9.7-8.5 17.6-18.7 17.6v-7.9c5.8 0 10.5-4.5 10.5-10.1 0-2.2 1.8-3.9 4.1-3.9s4.1 1.7 4.1 3.9z"/>
        <path class="st157" d="M1647.2 926.7v4.7h-7.7c3-1 5.6-2.6 7.7-4.7z"/>
        <path class="st157" d="M1651.4 913.3c-.2 9.7-8.5 17.6-18.7 17.6v-3.7c16.1.1 18.7-14 18.7-13.9z"/>
        <path class="st145" d="M1621.7 957.9h-11.3c0-2.5 4.9-4.6 11.3-5.1v5.1z"/>
        <path class="st157" d="M1629 932.8h11.9c.5.8-4 1.6-4 2.6 0 2.9-2.4 5.2-5.4 5.2-4.9 0-8.9 3.8-8.9 8.6v5h-8.6v-5c-.1-12.3 8.2-16.4 15-16.4z"/>
        <path class="st10" d="M1629 932.8h3.7c-.1 2.8-2.5 5-5.4 5-4.9 0-8.9 3.8-8.9 8.6v7.8h-4.5v-5c0-12.3 8.3-16.4 15.1-16.4z"/>
        <path class="st159" d="M1613.3 954.7c1.5.3 3.1 1.1 3.3 3.1h-6.2c0-1.1 1.1-2.2 2.9-3.1z"/>
        <path class="st145" d="M1631.8 957.9h-11.3c0-2.5 4.9-4.6 11.3-5.1v5.1z"/>
        <path class="st159" d="M1623.4 954.7c1.5.3 3.1 1.1 3.3 3.1h-6.2c0-1.1 1.1-2.2 2.9-3.1z"/>
        <path class="st157" d="M1639.1 932.8h7.9v2.6c0 2.9-2.4 5.2-5.4 5.2-4.9 0-8.9 3.8-8.9 8.6v5h-8.6v-5c-.1-12.3 8.2-16.4 15-16.4z"/>
        <path class="st10" d="M1639.1 932.8h3.7c-.1 2.8-2.5 5-5.4 5-4.9 0-8.9 3.8-8.9 8.6v7.8h-4.5v-5c0-12.3 8.3-16.4 15.1-16.4z"/>
        <path class="st154" d="M1628.2 958.9h2.4v6.6h-2.4z"/>
        <path class="st155" d="M1625.3 957.9h8.2v2h-8.2z"/>
        <path class="st154" d="M1611.6 958.9h2.4v6.6h-2.4z"/>
        <path class="st11" d="M1649.7 941.3h2.4v12.3h-2.4z"/>
        <path class="st152" d="M1606.7 957.9h18.6v2h-18.6z"/>
        <path class="st11" d="M1627.6 931.1h25.2v2.3h-25.2z"/>
        <path class="st155" d="M1630 931.1h18.3v3.4H1630z"/>
        <path class="st11" d="M1634 959.7c.7 0 1.2-.5 1.2-1.1v-11c0-1.9 1.6-3.4 3.5-3.4h8.1c3.9 0 7.1-3.1 7.1-6.8V921c0-1.3 1.1-2.3 2.4-2.3h6.2c.7 0 1.2-.5 1.2-1.1 0-.6-.5-1.1-1.2-1.1h-6.2c-2.6 0-4.7 2-4.7 4.6v16.4c0 2.5-2.1 4.6-4.7 4.6h-8.1c-3.3 0-5.9 2.6-5.9 5.7v11c-.1.4.4.9 1.1.9z"/>
        <path class="st159" d="M1629.3 968.7c2.5 0 4.5-1.9 4.5-4.3s-2-4.3-4.5-4.3-4.5 1.9-4.5 4.3c.1 2.4 2.1 4.3 4.5 4.3z"/>
        <path class="st155" d="M1657.3 915.8h8.7v3.2h-8.7z"/>
        <path class="st159" d="M1650.9 968.7c8.9 0 16.2-7 16.2-15.6s-7.3-15.6-16.2-15.6c-8.9 0-16.2 7-16.2 15.6s7.3 15.6 16.2 15.6zm0-28c7.1 0 12.9 5.6 12.9 12.4 0 6.8-5.8 12.4-12.9 12.4-7.1 0-12.9-5.6-12.9-12.4 0-6.8 5.8-12.4 12.9-12.4z"/>
        <path class="st159" d="M1650.9 951.2c1.1 0 2 .9 2 2s-.9 2-2 2-2-.9-2-2c-.1-1.2.9-2 2-2z"/>
        <path class="st159" d="M1651.1 967.7h-.4v-13.6l-5.7 12.5-.4-.2 5.6-12.4-9.9 9.5-.3-.3 10-9.6-13.2 4.9-.2-.4 13.1-4.9h-14v-.4h14.1l-12.9-5.5.2-.4 12.8 5.4-9.9-9.5.3-.3 10 9.6-5.1-12.7.4-.1 5.1 12.6v-13.5h.4V952l5.7-12.5.4.2-5.6 12.4 9.9-9.5.3.3-10 9.6 13.2-4.9.2.4-13.1 4.9h14v.4H1652l12.9 5.5-.2.4-12.8-5.4 9.9 9.5-.3.3-10-9.6 5.1 12.7-.4.1-5.1-12.6v13.5z"/>
        <path class="st141" d="M1675.4 915.2l-2.5-5.7v-8.2h4.2c2.3 0 4.2 1.8 4.2 4.1l2.5 13.9c0 2.3-1.9 4.1-4.2 4.1h-11.7v-8.2h7.5z"/>
        <path class="st11" d="M1665.5 918.8h-1.4c.3-.2.5-.4.7-.6.2.2.5.4.7.6z"/>
        <path class="st142" d="M1661.5 915.8c-1.8 1.8-1.8 4.6 0 6.4 1.8 1.8 4.8 1.8 6.6 0 1.8-1.8 1.8-4.6 0-6.4-1.8-1.7-4.7-1.7-6.6 0z"/>
        <path class="st143" d="M1661.7 920.5c1.8 1.8 4.8 1.8 6.6 0 .6-.5 1-1.2 1.2-1.9.1 1.3-.3 2.6-1.4 3.6-1.8 1.8-4.8 1.8-6.6 0-1.3-1.2-1.7-3-1.2-4.5.2 1 .6 2 1.4 2.8z"/>
        <path class="st141" d="M1667.9 915.2h5.4v8.2h-5.4z"/>
        <path class="st144" d="M1667.9 915.7v-.5h7v-5.9l3.8 9.7-3.8-3.3z"/>
        <path class="st144" d="M1668 919.6h11.7c1.6 0 3-.9 3.7-2.2l.4 1.8c0 2.3-1.9 4.1-4.2 4.1h-11.7v-8.2h.1v4.5z"/>
        <path class="st160" d="M1602.9 970.8c0 1.1.9 2 2.1 2h79.6c1.2 0 2.1-.9 2.1-2s-.9-2-2.1-2H1605c-1.2-.1-2.1.8-2.1 2z"/>
        <text transform="translate(1617.41 1014.675)">
          <tspan x="0" y="0" class="st92 st90 st94">Equal</tspan><tspan x="-32" y="24.5" class="st92 st90 st94">Opportunity</tspan>
        </text>
      </g>
    </g>
    <g id="guy-with-pin-2">
      <path class="st54 st67" d="M1400.9 3657.5c-.1-.1-.4-.2-.6-.2h-.1c-.1-.1-.2-.3-.5-.4-.4-.2-1.3-.5-2.9-.3-2 .3-2.5.5-2.1.8.3.2.8.4 1.1.5-.2 0-.1.1.1.2s.6.1.7.1c.1 0 .2.1.3.1.1 0 .3.1.4.1l.3.2-.5.2h.1l-.7.3s-1.3.2-1.4.3c-.6.4 1.3 1.8 1.3 1.8l.7.5 2.8.4 1.7.9.4-.1 3.9 2 4.2 2c.1.1.2.3.3.4.1.1.1.2.3.2.3 0 1.1 0 1.3-.1.3-.1.4-.3.4-.4 0-.1-.3-.2-.5-.3h.1l-1.4-.9-2-1.1-3.1-1.9 1.2-.1.9.5 2.4 1.4 1.7.8s1.9 1.1 2 1.1h.3c.1.1.3.2.5.2.2.1.8.2 1.1.2.5 0 1.6-.1 1.7-.2 0 0-.1-.1-.2-.1-.2-.1-.9-.3-1.1-.3l-2.9-2-3.8-2.3.4-.1-1.5-1 1.8-.8s-3.5-1.5-5.1-1.7c-.4-.1-1.6 0-1.6 0h-1.2l.1-.1-1.1-.1-.2-.1c.2-.1.3-.3.3-.3l-.1-.1c-.2 0-.1 0-.2-.2z"/>
      <path class="st84" d="M1416.9 3667.4c.1-.1 0-.3 0-.4-.1-.4-.4-1.5-.4-1.5h-1.6s-.1.7 0 .9c.1.3.3.8.5.9.4.2 1.3.3 1.5.1zm-4.5.1c.3-.1.7-.7.8-1 .1-.3 0-1.2 0-1.2h-1.3s-.3 1-.4 1.4c0 .2-.2.5-.1.7.1.2.7.2 1 .1z"/>
      <path class="st71" d="M1415.9 3638.7l-2.4-.5-.2 2.9h1.5l1.1-.8z"/>
      <path class="st77" d="M1415.8 3638.6c-1 .8-2.1-.1-2.1-.1s0 1.1.9 1.2c1.1.1 1.4-1.2 1.2-1.1z"/>
      <path class="st71" d="M1414.3 3639.2c.2.1.8.1 1.1 0 .4-.2 1-.8 1.2-1.2.2-.7 0-2.9 0-2.9h-3.4s-.1 2.2.1 2.9c.1.4.7 1 1 1.2z"/>
      <path class="st85" d="M1414.9 3635.3c.3 0 1.1.1 1.4.2.4.2.4 1.4.4 1.4s.3-.9.3-1.7c0-.7-.3-1.8-1.7-1.8-1.7 0-2.3.4-2.4 1.4-.1 1.1.3 2 .3 2s-.1-1.4.2-1.5c.2-.1 1.2 0 1.5 0z"/>
      <ellipse transform="rotate(-80.358 1416.693 3636.94)" class="st71" cx="1416.7" cy="3637" rx=".6" ry=".3"/>
      <ellipse transform="rotate(-9.7 1411.903 3636.373)" class="st71" cx="1413.1" cy="3637" rx=".3" ry=".6"/>
      <path class="st88" d="M1416.6 3665.7l.5-6.4.1-7.4h-6.2l.3 6.9.5 6.9h1.5l.2-2.9v-3.7l.1-6.1h1l.1 1.6-.1 4.6.1 2.8v3.7h1.9z"/>
      <path class="st69" d="M1414.1 3652.1l3.5-.2.2-3.2 2.2-1.4s-.5-5.2-1.4-6.3c-.2-.3-1.2-.5-1.2-.5l-1.3-.9s-.9.9-1.4.9c-.9-.1-1.1-1.4-1.1-1.4l-1.5.9s-1.1.1-1.4.4c-.9 1-1.3 5.2-1.3 5.2l-.2 1.6 1.5 1.9.1 3h3.3z"/>
      <path class="st161" d="M1416.8 3645.9l-1.7 1.7h1.1l1.4-1h.9l-.5-.4v-3.9zm-5.8.5l1.6 1.6.7-.1-1.5-2.1-.4-2.9-.6-1.1.2 3.5-.7.7z"/>
      <path class="st77" d="M1413 3648.4v.3l.7.6h1.2l.5-.3.8-.4v-1l-.9-.2-1.2-.3-.2.5.6.2-.4.2z"/>
      <path class="st71" d="M1414.8 3647.6l-1.2.2-1 .2v1.1l.9.4.4.3h1.2l.8-.6v-.3l-1.1-.4-.4-.2.6-.3z"/>
      <path class="st161" d="M1415.3 3641.2l1.4-1.4-.8-.6-1.3 1.3-1.1-1.6-.7.5.9 1.7.9-.4z"/>
      <circle class="st161" cx="1414.5" cy="3641.7" r=".1"/>
      <circle class="st161" cx="1414.5" cy="3643.2" r=".1"/>
      <circle class="st161" cx="1414.5" cy="3644.7" r=".1"/>
      <circle class="st161" cx="1414.5" cy="3646.1" r=".1"/>
      <circle class="st161" cx="1414.2" cy="3650.8" r=".1"/>
      <path class="st11" d="M1413.9 3586.9c-3.7 2.2-6.7 7.4-6.7 11.7 0 4.3 3 6 6.8 3.9 3.7-2.2 6.7-7.4 6.7-11.7 0-4.4-3-6.1-6.8-3.9z"/>
      <path class="st162" d="M1425.9 3587.9c0 7.6-11.3 34.4-11.9 35.8-.6-.7-12-14.4-12.1-22 0-7.6 5.3-16.8 11.9-20.7 6.7-3.7 12.1-.7 12.1 6.9zm-11.9 14.5c3.7-2.2 6.7-7.4 6.7-11.7 0-4.3-3-6-6.8-3.9-3.7 2.2-6.7 7.4-6.7 11.7 0 4.3 3.1 6 6.8 3.9z"/>
      <path class="st163" d="M1407 3577c3.3-1.9 6.3-2.1 8.5-.8 2.3 1.3 4.6 2.7 7 4-2.2-1.3-5.2-1.1-8.5.8-6.6 3.8-11.9 13.1-11.9 20.7s11.4 21.2 12.1 22l-7-4c-.6-.7-12-14.4-12.1-22-.1-7.6 5.3-16.8 11.9-20.7z"/>
    </g>
    <g id="guy-with-pin-1">
      <path class="st11" d="M1455.7 2444.2c-3.7 2.2-6.7 7.4-6.7 11.7 0 4.3 3 6 6.8 3.9 3.7-2.2 6.7-7.4 6.7-11.7 0-4.4-3-6.1-6.8-3.9z"/>
      <path class="st162" d="M1467.7 2445.2c0 7.6-11.3 34.4-11.9 35.8-.6-.7-12-14.4-12.1-22 0-7.6 5.3-16.8 11.9-20.7 6.7-3.7 12.1-.7 12.1 6.9zm-11.9 14.5c3.7-2.2 6.7-7.4 6.7-11.7 0-4.3-3-6-6.8-3.9-3.7 2.2-6.7 7.4-6.7 11.7 0 4.3 3 6 6.8 3.9z"/>
      <path class="st163" d="M1448.8 2434.3c3.3-1.9 6.3-2.1 8.5-.8 2.3 1.3 4.6 2.7 7 4-2.2-1.3-5.2-1.1-8.5.8-6.6 3.8-11.9 13.1-11.9 20.7s11.4 21.2 12.1 22l-7-4c-.6-.7-12-14.4-12.1-22-.1-7.6 5.2-16.9 11.9-20.7z"/>
      <path class="st54 st67" d="M1446.6 2518.8s.8-.1.4-.5c-.1-.1-.8-.3-1.3-.4h-1.1s-.7-.1-1.6 0c-1 .2-1.6.5-1.2.7.1.1.6.1.8.2.2.1 1 .2 1 .2l.1-.1c.3.1.6.1.9.2h.1-.3l-.9.2-.4.1-.3.1-.3.2c0 .1.9.5.9.5s.7.5 1 .6c.4.2 1.7.6 1.7.6l.8.2.4.1h.1l.4.1.6.1.3.2 1.3.9.6.5v.2l.5.8-.1.2.3.3h-.1l.1.1h.1c-.1.1-.3.2-.7.3-.2 0 .1.3 1.5.2.3 0 .6-.1.8-.2.4-.1 1.6-.1 1.7-.2l-.2-.1-.4-.1h.1l-.4-.1.2-.5-.4-.5-.4-.5v-.2l-.3-.4-.9-.8h.4l2.6.8.7.5.4.1 1.9 1 .6.1c.2.1.5.2.6.2.1 0 .1.1.3.1.3 0 .9 0 1.1-.1.3 0 .8-.1.9-.2 0-.1-.4-.1-.6-.2-.1 0-.3-.2-.3-.2l.1-.3-1.2-.5-.9-.5-.6-.2-1.3-.7-1-.4-.6-.3c.2-.1.3-.2.5-.2h.4c.1 0 .1-.1.1-.1-.1-.1-.4-.2-.7-.3l-1.8-.5c.2-.1.6-.2.7-.2.1-.1-.2-.3-.2-.3l-.8-.3s-1.5-.4-2-.5c-.6-.1-1.4-.1-1.4-.1h-3.3v.1z"/>
      <path class="st68" d="M1452.1 2526.1c.1.2.7.3 1 .3.3 0 .9 0 1-.2.1-.1 0-.5 0-.6 0-.3.1-1.3.1-1.3l-1.2-.4-.7.7s.1.6 0 .8c0 0-.3.5-.2.7zm8.5-.3c.2 0 .7.3 1 .3 1.4 0 2.1-.4 2.1-.4s-.1-.4-.2-.5c-.2-.2-.7-.2-.9-.3-.7-.3-1.2-1-1.2-1l-2.3.6-.2.7s-.1.3 0 .4c.2.3 1.2.1 1.7.2z"/>
      <path class="st69" d="M1452 2521.3l-.2 2.3.5.9s.9-.4 1.2-.4c.2 0 .8.2.8.2l.4-.5v-4.5l.2-.6-.2-2.1 1-3.9h.4l.6 3.5.3 1.5.3.7.5 2.1.4 2 .9 1.7-.2.5s1.2.3 1.5.2c.3-.1 1.1-.8 1.1-.8l-.1-.5h-.1l-.2-1.3-.4-.8-.9-3.2-.2-.7-.3-2-.4-3.9-.2-1.7-2.2-.2-3.1-1.3-1.2 2.3v2l-.2 1.9.1 3.3-.1 1.1v2.2z"/>
      <path class="st70" d="M1454.1 2508.7l-.9.7-.7 5.1.3 2.6.7.1.5-.8 1.2-3.8-.8-1 .9.4.8.1 1.1-.1-.7.3 1.3 5.4.5.2.6-.2-.4-5.1-.1-1.8-.4-.2-.4-1-1.1-.2-.4 1.8-.5-.2.2-1.8z"/>
      <path class="st71" d="M1459.5 2509.5l-1.2-.4.5 1.8.4-.6zm-1.8-10.3l-.4-.2-.1-1-1.9.1v.8l-.5.2-.1 1.9 2.8.7.3-1.6z"/>
      <path class="st71" d="M1458 2496.6c0-1.2-.8-1.7-1.7-1.7-.9 0-1.7.5-1.7 1.7s.8 2.8 1.7 2.8c1 0 1.7-1.6 1.7-2.8z"/>
      <path class="st72" d="M1460.3 2500.7c-.1-.3-.6-.8-.6-.8l-.9 2.2-.4 7.1 1.1.6.2-.4.3-1.1s.5-2 .5-2.7c0-.6-.1-2.6-.1-2.6s.1-1.8-.1-2.3z"/>
      <path class="st73" d="M1452.5 2508.8s2.2.9 3.7 1.1c.5.1 2.4.1 2.4.1l.1-1s.3-.6.3-.8c.2-1.2-.1-3.6.1-4.8.1-.4.4-1.1.4-1.4.1-.5.1-2 .1-2l-2.2-.8s.2 1.8-.8 1.9c-1.5.2-1.9-1.9-1.9-1.9-1.8.4-2.2.9-2.2.9s.7 1.4.8 2c.1.7-.5 2.7-.5 2.7l-.3 4z"/>
      <path class="st74" d="M1457.5 2506.7c.9-1.2 1.1-4.3 1.3-5.7v-1.4l-1.1-.4s0 1.1-.1 1.6c-.1 1.3-.1 3.9-.7 5-.4.7-2.6 2.1-2.6 2.1l.1 1c-.1 0 2.6-1.5 3.1-2.2z"/>
      <path class="st75" d="M1453.1 2506.4l-1.2.3-.8 2.8.5.6 2.6-2.5z"/>
      <path class="st71" d="M1457.1 2507.6c.1 0 .2-.2.2-.2s.2-.1.2-.2.1-.3.1-.3l.1-.1c0-.1.1-.3.1-.3l.2-.2c0-.1-.2-.4-.2-.4l-.8-.2-.1-.2h-.2c-.2.1-.4.3-.6.4h-.5l-.2 1.2.4.1s.5.4.7.4c.1.1.5.1.6 0z"/>
      <path class="st76" d="M1458 2498.2s.4-1 .4-1.3c.1-.3.4-.8.3-1.1-.1-1.1-1.1-2.1-2.2-2.2-1-.2-1.4.5-1.4.5s-.7.4-.8.6c-.3.4-.6 1.3-.5 1.8.2 1.3 1.1 1.5 1.1 1.5s-.3-1.5-.1-1.4c.2.1.5.1.5.1s-.4-1.2-.2-1c.4.3 1.5.7 1.5.7l-.1-.9s1 .6 1.3 1.2c.1.3 0 .8 0 1.1 0 .3.2.4.2.4z"/>
      <path class="st72" d="M1453.5 2502c-.1-1.6-.9-2-.9-2s-.6.4-1 1.1c-.3.6-.8 2.8-.8 2.8l-.2 1.4s0 .8.2 1c.2.2.8.6 1.1.6.3.1.8.2 1 .3.6.1 2.5 0 2.5 0l.3-1.2-2.9-.8c0-.2.3-1.2.3-1.2s.5-1 .4-2z"/>
      <path class="st77" d="M1457.1 2499s-.7.8-1.4.1c-.1-.1.1 1 .8.9.6-.1.6-1 .6-1z"/>
      <path class="st70" d="M1461.3 2523.4l-1.2.5-.8.2.9.1 1.3-.7zm-8.2-.6l-1 .8.9-.4 1.5.6z"/>
      <path class="st78" d="M1456.6 2500.6c-1.1.2-1.5-1.7-1.5-1.7l-.3.1s.4 2.1 1.9 2c1.1-.1.8-1.9.8-1.9l-.2-.1s.1 1.5-.7 1.6zm2 9.4v-1s-1.9 0-2.5-.1c-.5-.1-1.9-.5-1.9-.5l-.3 1s.7.3 2.1.6c.7.1 2.6 0 2.6 0z"/>
      <path class="st74" d="M1451.2 2511.2c.1 0 .2-.2.3-.2.3 0 .6.6.9.5.9-.1 2.3-2.9 2.3-2.9s.3-.9-.5-1c-.9-.1-2.6 1.1-3.1 1.8-.2.3-.2 1-.2 1.3.1.2.2.5.3.5z"/>
      <path class="st78" d="M1453.4 2503.9c.4-.4.6-1.3.5-2.3-.2-1.7-.9-1.8-.9-1.8l-.3.3s.6.3.8 1.5c.2 1.3-.3 2.5-.3 2.5l.2-.2zm5.7-.6s.3-.9.4-1.3c.1-.5.1-2.1.1-2.1l-.4-.2v1.6c0 .6-.1 2-.1 2z"/>
    </g>
    <g id="daytime-hours">
      <text transform="translate(194.91 1310.572)">
        <tspan x="0" y="0" class="st89 st90 st91">Daytime Hours</tspan><tspan x="364.1" y="0" class="st89 st90 st164"></tspan>
      </text>
      <text transform="translate(194.91 1348.796)">
        <tspan x="0" y="0" class="st92 st93 st165">During the day this is an appointment-based mean of </tspan><tspan x="0" y="24.5" class="st92 st93 st165">transportation with service focused specifically on individuals</tspan><tspan x="0" y="49" class="st92 st93 st165">with disabilities (temporary or permanent), military veterans</tspan><tspan x="0" y="73.4" class="st92 st93 st165">and faculty and staff.</tspan>
      </text>
      <g id="daytime-icon-1">
        <defs>
          <circle id="SVGID_1_" cx="265.7" cy="1530.5" r="57.1"/>
        </defs>
        <use xlink:href="#SVGID_1_" overflow="visible" opacity=".56" fill="#FFF"/>
        <clipPath id="SVGID_2_">
          <use xlink:href="#SVGID_1_" overflow="visible" opacity=".56"/>
        </clipPath>
        <g class="st166">
          <path class="st167" d="M280.9 1510.1c3.6-9.8 7.7-18.3-6.4-22.3-14.1-3.9-6.7-5.5-6.7-5.5s-11-6-17.8 2.8c-6.8 8.8-2.5 25-2.5 25h33.4z"/>
          <path class="st168" d="M291.5 1587.4c.1-11.2.5-24.8 1.1-27.7 1.9-8.9 7.2-8.8 6.8-13.4-.9-9.7-20.3-18.7-35.7-17.3-15.4 1.5-36 10.5-26.2 20.2 3.7 3.7 2.7 2.5 4.7 12.8.5 2.3 1.1 14.7 1.6 25.3h47.7z"/>
          <path class="st169" d="M294.9 1587.4c1.7-4.9 4-7.3 8.7-5.6.9.3 2.3 2.3 1.8 5.6h-10.5z"/>
          <path class="st170" d="M305.4 1587.4c.6-3.3-.9-5.3-1.8-5.6-.1 0-.2-.1-.2-.1 1.3 1.3 1.4 3.4.8 5.7h1.2z"/>
          <path class="st168" d="M308.7 1587.4c1.7-4 2.9-6.4 2.9-6.4 1.4-3.9-.8-8.2-4.8-9.7-4.1-1.4-8.5.5-9.9 4.4 0 0-1.9 4.7-4.3 11.6h16.1z"/>
          <path class="st168" d="M288.6 1539.2c-4 1.6-6.1 6-4.6 9.8l12.3 31.5c1.5 3.9 6 5.7 10 4.2 4-1.6 6.1-6 4.6-9.8l-12.3-31.5c-1.5-3.9-5.9-5.8-10-4.2z"/>
          <path class="st169" d="M238.6 1587.4c-1.7-5.2-4-7.9-8.8-6.1-1 .4-2.5 2.5-1.7 6.1h10.5z"/>
          <path class="st170" d="M228 1587.4c-.8-3.6.7-5.8 1.7-6.1.1 0 .2-.1.2-.1-1.4 1.4-1.4 3.7-.6 6.2H228z"/>
          <path class="st168" d="M243.3 1537.1c4.3.1 7.4 3 7.1 6.6l-2.9 29.3c-.4 3.6-4.1 6.4-8.4 6.4-4.3-.1-7.4-3-7.1-6.6l2.9-29.3c.4-3.7 4.1-6.5 8.4-6.4z"/>
          <path class="st171" d="M276.2 1533c0 8.3-19.6 8.3-19.6 0v-19c0-3.8 3-6.8 6.8-6.8h6c3.8 0 6.8 3 6.8 6.8v19z"/>
          <path class="st172" d="M247.4 1514.6c.2 1.1 1.3 1.9 2.5 1.7 1.2-.2 2-1.2 1.9-2.3l-.9-6.1c-.2-1.1-1.3-1.9-2.5-1.7-1.2.2-2 1.2-1.9 2.3l.9 6.1z"/>
          <path class="st173" d="M249.3 1512.1c.1.4.4.7.8.6.4-.1.7-.4.6-.8l-.5-3.5c-.1-.4-.4-.7-.8-.6-.4.1-.7.4-.6.8l.5 3.5z"/>
          <path class="st171" d="M283.8 1515.2c-.2 1.1-1.3 1.9-2.5 1.7-1.2-.2-2-1.2-1.9-2.3l.9-6.1c.2-1.1 1.3-1.9 2.5-1.7 1.2.2 2 1.2 1.9 2.3l-.9 6.1z"/>
          <path class="st173" d="M281.9 1512.7c-.1.4-.4.7-.8.6-.4-.1-.7-.4-.6-.8l.5-3.6c.1-.4.4-.7.8-.6.4.1.6.4.6.8l-.5 3.6z"/>
          <path class="st167" d="M264.1 1495.9c14.9 0 15.8 9.5 15.8 9.5.7 2.4 1.1 4.9 1.1 7.6 0 11.4-6.9 20.7-15.5 20.7-8.5 0-15.5-9.3-15.5-20.7 0-4.6-1.1-13.8.7-17.2 2.4-4.5 7.9.4 13.4.1z"/>
          <path class="st172" d="M264.1 1495c14.9 0 13.2 9.5 13.3 9.5.7 2.4 2.4 4.9 2.4 7.6 0 11.4-5.7 13.9-14.2 13.9s-13.5-2.8-13.5-14.2c0-4.6-2.7-12-.8-15.4 2.3-4.6 7.3-1.1 12.8-1.4z"/>
          <path class="st167" d="M254.8 1508.6c0 .7 1.6.4 3.5.5 2 .1 3.5.5 3.6-.2 0-.7-1.5-1.3-3.5-1.4-1.9-.1-3.6.4-3.6 1.1z"/>
          <path class="st174" d="M255.5 1508.6c0-.6 1.3-.2 3-.2 1.6.1 3-.2 3 .4 0 .6-1.4 1-3 .9-1.7 0-3.1-.5-3-1.1z"/>
          <ellipse class="st167" cx="258.2" cy="1508.5" rx="1" ry=".9"/>
          <path class="st171" d="M265.2 1495c9.3.7 15.2-2.9 14.5 8.3-.3 4.1.5 6.4.5 9.1 0 11.4-6 14.7-14.6 14.7h-.4V1495z"/>
          <path class="st167" d="M269.3 1509.2c0 .7 1.6.4 3.5.5 2 .1 3.5.5 3.6-.2 0-.7-1.5-1.3-3.5-1.4-1.9-.1-3.5.4-3.6 1.1z"/>
          <path class="st174" d="M270 1509.2c0-.6 1.3-.2 3-.2 1.6.1 3-.2 3 .4 0 .6-1.4 1-3 .9-1.7 0-3.1-.5-3-1.1z"/>
          <ellipse class="st167" cx="272.7" cy="1509.1" rx="1" ry=".9"/>
          <path class="st172" d="M266.9 1508.5c.5 4.1 2 6.4 2 8 0 1.7-1.7 2.9-3 2.9s-4.2-1-3.6-3.5c.6-2.5 1.8-6.5 1.8-7.4 0-1.6 2.7-1.6 2.8 0z"/>
          <path class="st171" d="M266.7 1514.9c-1.2-4.2-1.5-7.6-1.5-7.6.9-.3 1.8 0 1.9.9.5 4.1 1.8 6.6 1.8 8.3 0 1.7-1.7 2.9-3 2.9-.2 0-.5 0-.7-.1 0 0 2.7-.3 1.5-4.4z"/>
          <path class="st167" d="M257.8 1524.5c-.1 3.6 3.3 7 7.4 7.3 4 .2 7.1-2.9 7.2-6.4.1-3.6-.7-6.5-7.1-6.9-6.5-.4-7.4 2.4-7.5 6z"/>
          <path class="st172" d="M260 1524.2c-.1 2.3 2.7 1 5.5 1.1 2.8.1 4.5 1.7 4.6-.6.1-2.3-.4-4.2-4.9-4.5-4.5-.2-5.1 1.6-5.2 4z"/>
          <path class="st175" d="M268 1522.7c0-.4-1.4-.2-3-.3-1.7-.1-3-.3-3.1.1 0 .4 1.3.8 3 .8 1.7.1 3.1-.2 3.1-.6z"/>
          <path class="st176" d="M271.2 1562.4l-4.5 2.8-20.7-31.6 6-2.2z"/>
          <path class="st169" d="M265.6 1573.6c11.1-2.1 18.1-1.3 16.7-4.5-.9-2.1 1.8-1.8.7-3.9-1.1-2.2 1.2-1.5-.5-3.9-2.2-3.1.7-1.3-1.2-3.8-2-2.5-7.4 1.3-10.7.6-1.1-.2-1.5.4-1.7 1.4-.4 1.9-.5 5.1-4.9 6.7-7 2.3-1.4 8 1.6 7.4z"/>
          <path class="st170" d="M268.9 1558.7c.9 4.4-.7 6.9-4.1 8.4-1.5.5-4 .3-4.8.1.4-.8 2.2-.6 3.7-1.2 4.5-1.5 4.5-4.8 4.9-6.7.2-.2.3-.4.3-.6z"/>
          <path class="st176" d="M275.8 1564.6c.8 3.9-1.6 7.6-5.3 8.4l-30.4 6.2c-3.7.8-7.4-1.8-8.2-5.6-.8-3.9 1-18.4 2.7-26.8l33 12.2c3.7-.8 7.4 1.8 8.2 5.6z"/>
          <path class="st167" d="M277.2 1506.4c-4.7-2-8 1.8-8.5.5-.3-.9 1.6-1.6 4-1.7 2.3-.1 4 .3 4.5 1.2zm-23.9-.9c5-1.6 8.1 2.7 8.7 1.4.4-.9-1.5-1.8-3.9-2.2-2.4-.4-4.2-.1-4.8.8z"/>
          <path class="st177" d="M278.7 1507.6c0-.4-.1-.5-.5-.5s-.7-.8-1.5-.8-6.3.1-8.2.2c-1.9.1-1.8 1.5-3.3 1.5-1.5 0-1.4-1.5-3.3-1.5-1.9-.1-7.4-.2-8.2-.2-.8 0-1.1.8-1.5.8-.4 0-.5.1-.5.5v1.4c0 .6.5.3.7.8.2.5.6 2.2 1.9 2.3 1.4.1 4.8 0 6.6.1 1.8.1 2.2-.7 2.7-1.8.5-1 .9-1.5 1.6-1.5.8 0 1.1.5 1.6 1.5s.9 1.9 2.7 1.8c1.8-.1 5.3-.1 6.6-.1 1.3-.1 1.7-1.7 1.9-2.3.2-.5.7-.2.7-.8.1-.5 0-1 0-1.4zm-15.8 2.8c-.5 1-.3 1.6-3.5 1.5-3.3-.1-4.8.2-5.7-.5-.9-.7-.8-1.4-.8-2.4 0-1.1-.1-2.1 1.2-2.1h6.8c1.2 0 1.6.4 1.9.7.7.7.7 1.7.1 2.8zm13.8 1c-.9.7-2.4.4-5.7.5-3.3.1-3-.5-3.5-1.5s-.6-2.1.1-2.8c.2-.3.7-.7 1.9-.7 1.3 0 5.5-.1 6.8 0 1.3 0 1.2 1.1 1.2 2.1.1 1 .1 1.7-.8 2.4z"/>
        </g>
        <text transform="translate(209.76 1618.557)" class="st92 st90 st178">
          Disabilities
        </text>
      </g>
      <g id="daytime-icon-2">
        <defs>
          <circle id="SVGID_3_" cx="464.6" cy="1530.5" r="57.1"/>
        </defs>
        <use xlink:href="#SVGID_3_" overflow="visible" opacity=".56" fill="#FFF"/>
        <clipPath id="SVGID_4_">
          <use xlink:href="#SVGID_3_" overflow="visible" opacity=".56"/>
        </clipPath>
        <g class="st179">
          <defs>
            <circle id="SVGID_5_" cx="464.7" cy="1532" r="58.1"/>
          </defs>
          <use xlink:href="#SVGID_5_" overflow="visible" opacity=".56" fill="#FFF"/>
          <clipPath id="SVGID_6_">
            <use xlink:href="#SVGID_5_" overflow="visible" opacity=".56"/>
          </clipPath>
          <g class="st180">
            <path class="st181" d="M410 1574.8c-5.8 7.7 5.2 16.7 12.2 10.1l25.1-23.4c8.4-11.8-9.3-24.6-16.9-13.9l-20.4 27.2z"/>
            <path class="st182" d="M426.6 1576.5c4.2-3.1 7.9-7.1 11.5-10.8 2.2-2.2 3.8-5 5.6-7.5 1.2-1.8 2.4-3.4 3.2-5.3.4-1.1.8-2.1 1.1-3.2 2 3.3 2.3 7.7-.7 11.9l-25.1 23.4c-4 3.8-9.3 2.4-12.1-.8 1.8-.2 3.6-.6 5.1-1.3 4.2-2 7.9-3.8 11.4-6.4z"/>
            <path class="st181" d="M499.8 1593.6c3.4-1 6.2-4.1 5.6-8.5l-4.2-32.6c-4.6-13.2-25.4-6.8-21.2 5.1l10.1 31.2c.8 2.6 2.6 4.1 4.6 4.8h5.1z"/>
            <path class="st182" d="M497.9 1593.6c.8-1.4 1.4-2.9 1.7-4.3.9-4.1 1.6-8.1 1.6-12.2 0-5-1.2-10.1-2-15-.5-2.9-1.8-5.8-2.8-8.6-.7-2-1.4-3.8-2.5-5.5-.6-1-1.3-1.8-1.9-2.7 3.9.4 7.6 2.6 9.2 7.3l4.2 32.6c.6 4.4-2.2 7.4-5.6 8.5h-1.9z"/>
            <path class="st181" d="M490.9 1593.6c.9-11.5 7.5-31.7 7.5-39 0-10-16.7-18.1-32.4-18.1s-33 5.8-33 15.8c0 7.3 7.2 29.5 8.1 41.3h49.8z"/>
            <ellipse class="st182" cx="465.8" cy="1541.2" rx="12.5" ry="6.6"/>
            <path class="st171" d="M475.1 1540.4c0 7.9-18.5 7.9-18.5 0v-17.9c0-3.5 2.9-6.4 6.4-6.4h5.6c3.5 0 6.4 2.9 6.4 6.4v17.9z"/>
            <path class="st183" d="M444 1521.9c0 4.2 9.7 7.6 21.6 7.6 11.9 0 21.6-3.4 21.6-7.6 0-4.2-10-14.1-22-14.1-11.9 0-21.2 9.9-21.2 14.1z"/>
            <path class="st172" d="M448 1522.1c.1 1 1.2 1.8 2.3 1.6 1.1-.2 1.9-1.1 1.8-2.2l-.8-5.7c-.2-1-1.2-1.8-2.3-1.6-1.1.2-1.9 1.1-1.8 2.2l.8 5.7z"/>
            <path class="st173" d="M449.7 1520.7c.1.4.4.7.8.6.4 0 .6-.4.6-.8l-.5-3.3c-.1-.4-.4-.7-.8-.6-.4.1-.6.4-.6.8l.5 3.3z"/>
            <path class="st171" d="M482.3 1523.6c-.1 1-1.2 1.8-2.3 1.6-1.1-.2-1.9-1.1-1.8-2.2l.8-5.7c.2-1 1.2-1.8 2.3-1.6 1.1.2 1.9 1.1 1.8 2.2l-.8 5.7z"/>
            <path class="st173" d="M480.5 1521.2c-.1.4-.4.7-.8.6-.4-.1-.6-.4-.6-.8l.5-3.3c.1-.4.4-.7.8-.6.4.1.6.4.6.8l-.5 3.3z"/>
            <path class="st173" d="M454.2 1509.8c3.5 0 6.8-.9 9.6-2.5 3.3 4.1 8.6 6.8 14.7 6.8h.3c.7 2.2 1 4.6 1 7.2 0 10.8-6.5 19.5-14.6 19.5s-14.6-8.7-14.6-19.5c0-4.3 1-8.3 2.8-11.5h.8z"/>
            <path class="st172" d="M454.2 1509.1c3.5 0 6.8-.9 9.6-2.5 3.3 4.1 8.6 6.8 14.7 6.8h.3c.7 2.2 1 4.6 1 7.2 0 10.8-6.5 19.5-14.6 19.5s-14.6-8.7-14.6-19.5c0-4.3 1-8.3 2.8-11.5h.8z"/>
            <path class="st184" d="M455 1517.4c0 .7 1.5.4 3.3.4 1.8.1 3.3.5 3.4-.2 0-.7-1.4-1.3-3.3-1.3s-3.4.4-3.4 1.1z"/>
            <path class="st174" d="M455.6 1517.4c0-.5 1.3-.2 2.8-.2 1.5.1 2.8-.2 2.8.4 0 .5-1.3.9-2.8.9-1.6-.1-2.8-.5-2.8-1.1z"/>
            <ellipse class="st184" cx="458.1" cy="1517.3" rx="1" ry=".8"/>
            <path class="st171" d="M464.8 1507.8c3.3 3.5 8.2 5.6 13.7 5.6h.3c.7 2.2 1 4.6 1 7.2 0 10.8-6.5 19.5-14.6 19.5h-.4v-32.3z"/>
            <path class="st184" d="M468.7 1518c0 .7 1.5.4 3.3.4 1.8.1 3.3.5 3.4-.2 0-.7-1.4-1.3-3.3-1.3-1.9-.1-3.4.4-3.4 1.1z"/>
            <path class="st174" d="M469.3 1518c0-.5 1.3-.2 2.8-.2 1.5.1 2.8-.2 2.8.4 0 .5-1.3.9-2.9.9-1.5-.1-2.8-.6-2.7-1.1z"/>
            <ellipse class="st184" cx="471.8" cy="1517.8" rx="1" ry=".8"/>
            <path class="st171" d="M459.8 1531.4c-.1 1.9 2.8.8 5.7.9 2.9.1 4.6 1.4 4.7-.5.1-1.9-.4-3.5-5-3.7-4.6-.2-5.3 1.4-5.4 3.3z"/>
            <path class="st175" d="M461.2 1530.2c0 .5 1.6.3 3.6.4 2 .1 3.6.4 3.7-.1 0-.5-1.6-.9-3.6-1-2-.1-3.6.2-3.7.7z"/>
            <path class="st172" d="M466.4 1517.3c.4 3.9 1.9 6 1.9 7.6 0 1.6-1.6 2.7-2.8 2.7-1.2 0-4-1-3.4-3.3.6-2.3 1.7-6.1 1.7-7-.1-1.5 2.4-1.5 2.6 0z"/>
            <path class="st173" d="M466.2 1523.4c-1.2-4-1.1-7.1-1.1-7.1.9-.3 1.2-.1 1.3.8.4 3.9 1.9 6.2 1.9 7.8 0 1.6-1.6 2.7-2.8 2.7-.2 0-.4 0-.7-.1 0 0 2.5-.3 1.4-4.1z"/>
            <path class="st172" d="M445.8 1521c.2 1.2 1.3 2 2.6 1.8 1.3-.2 2.2-1.3 2-2.5l-.9-6.5c-.2-1.2-1.3-2-2.6-1.8-1.3.2-2.2 1.3-2 2.5l.9 6.5z"/>
            <path class="st173" d="M447.8 1518.3c.1.4.4.7.9.7.4-.1.7-.5.6-.9l-.6-3.8c-.1-.4-.4-.7-.9-.7-.4.1-.7.5-.6.9l.6 3.8z"/>
            <path class="st171" d="M484.5 1521.6c-.2 1.2-1.3 2-2.6 1.8-1.3-.2-2.2-1.3-2-2.5l.9-6.5c.2-1.2 1.3-2 2.6-1.8 1.3.2 2.2 1.3 2 2.5l-.9 6.5z"/>
            <path class="st173" d="M482.5 1518.9c-.1.4-.4.7-.9.7-.4-.1-.7-.5-.6-.9l.6-3.8c.1-.4.4-.7.9-.7.4.1.7.5.6.9l-.6 3.8z"/>
            <path class="st172" d="M452.8 1505.3c4 0 7.6-1 10.8-2.8 12.6-6 9.7 7.6 16.6 7.6h.3c.7 2.5 1.1 5.2 1.1 8.1 0 12.2-7.4 22-16.4 22-9.1 0-16.4-9.9-16.4-22 0-4.8 1.2-9.3 3.1-13 .3.1.6.1.9.1z"/>
            <path class="st185" d="M453.7 1514.6c0 .8 1.7.4 3.7.5 2.1.1 3.7.5 3.8-.2 0-.8-1.6-1.4-3.7-1.5-2.1-.1-3.8.5-3.8 1.2z"/>
            <path class="st174" d="M454.4 1514.6c0-.6 1.4-.2 3.2-.2 1.7.1 3.2-.2 3.1.4 0 .6-1.5 1-3.2 1-1.8 0-3.1-.6-3.1-1.2z"/>
            <ellipse class="st185" cx="457.3" cy="1514.5" rx="1.1" ry=".9"/>
            <path class="st171" d="M464.6 1502.4c16.3-8.7 17.1 7.7 17.2 7.7.7 2.5-.1 5.1-.1 8 0 12.2-7.4 22-16.4 22h-.4l-.3-37.7z"/>
            <path class="st185" d="M469.1 1515.3c0 .8 1.7.4 3.7.5 2.1.1 3.7.5 3.8-.2 0-.8-1.6-1.4-3.7-1.5-2-.1-3.8.4-3.8 1.2z"/>
            <path class="st174" d="M469.8 1515.3c0-.6 1.4-.3 3.2-.2 1.7.1 3.2-.2 3.1.4 0 .6-1.5 1-3.2 1-1.7-.1-3.1-.6-3.1-1.2z"/>
            <ellipse class="st185" cx="472.7" cy="1515.1" rx="1.1" ry="1"/>
            <path class="st173" d="M465.2 1540.2c-8 0-14.7-7.7-16.1-17.8 1 .9 3.2 2.8 6.6 3.7 2.6.7 4.5-.9 8.7-1.2 3.7-.2 5.9 1.4 8.4.9 4.3-.9 6.5.2 8.6-3.5-1.6 10.3-8.2 17.9-16.2 17.9z"/>
            <path class="st186" d="M464.7 1525c3.4-.1 5.5 1.4 8 .9 4.3-.9 7.1-.8 8.6-3.5-1.5 10.2-8.1 17.8-16.1 17.8h-.4c3.1-1.8-.1-15.2-.1-15.2z"/>
            <path class="st171" d="M469.9 1529.1c.1-2-2.8-.8-5.8-.9-2.9-.1-4.7-1.4-4.8.5-.1 2 .4 3.6 5.1 3.7 4.7.2 5.4-1.4 5.5-3.3z"/>
            <path class="st175" d="M468.5 1530.3c0-.5-1.7-.3-3.7-.4-2.1-.1-3.7-.4-3.7.1s1.6.9 3.7 1c1.9.1 3.6-.2 3.7-.7z"/>
            <path class="st172" d="M466.6 1514.5c.5 4.4 2.1 6.8 2.1 8.6 0 1.8-1.8 3-3.2 3-1.3 0-4.5-1.1-3.8-3.7.7-2.6 1.9-6.9 1.9-7.8 0-1.8 2.8-1.8 3-.1z"/>
            <path class="st173" d="M466.3 1521.3c-1.3-4.5-1.3-8-1.3-8 1-.3 1.3-.1 1.4.9.5 4.4 2.2 7 2.2 8.8 0 1.8-1.8 3-3.2 3-.2 0-.5 0-.8-.1.1.1 3-.3 1.7-4.6z"/>
            <path class="st183" d="M480.7 1510.3c.6 2 .8 4.2.8 6.3 0 11.1-7.5 20.1-16.7 20.1s-16.7-9-16.7-20.1c0-2.2.3-4.3.8-6.3l-2.2-.6c-.6 2.2-.9 4.6-.9 6.9 0 12.3 8.5 22.4 19 22.4s19-10 19-22.4c0-2.4-.3-4.7-.9-6.9l-2.2.6z"/>
            <path class="st181" d="M443.7 1521.1c-.7-2.6-1.1-5.4-1.1-8.3 0-14.6 10.4-22.8 23.1-22.8 12.8 0 23.1 8.2 23.1 22.8 0 2.9-.4 5.7-1.1 8.3-4.6 0-3.4-8.9-9.2-8.9h-25.3c-5.7 0-4.5 8.9-9.2 8.9h-.3z"/>
            <path class="st181" d="M443.7 1521.1h.4c1.6 0 2.4-1 3.2-2.3-1.4.1-2.7.2-4.1.3.1.6.3 1.3.5 2z"/>
            <path class="st182" d="M477.5 1492.7c3.6 3.8 4.6 9.4 1.1 13.7-1.8 2.3-3.8 4.2-6 5.7h5.9c5.7 0 4.5 8.9 9.2 8.9.7-2.6 1.1-5.4 1.1-8.3 0-9.6-4.6-16.4-11.3-20z"/>
            <path class="st184" d="M476.4 1534c1 1.4-3.8 5.9-11.4 5.9-7.6 0-12.4-4.5-11.4-5.9.9-1.5 5.8-.2 11.4-.3 5.6.1 10.5-1.2 11.4.3zm-28.5 59.6c-3.1-17.8-8.9-51.8-8.9-51.8l6.7-1.2s6.1 35.6 9.1 53h-6.9zm24.7 0c3.1-17.6 9.3-52.4 9.3-52.4l6.7 1.2s-5.9 33.3-9.1 51.2h-6.9z"/>
            <path class="st183" d="M429.6 1542.8c7.5 1.3 19.5-5.3 19.5-5.3l.6 1.3s-11.5 6.6-16.6 7.4c-5 1-3.5-3.4-3.5-3.4zm70.9 1c-7.5 1.3-19.5-5.3-19.5-5.3l-.6 1.3s11.5 6.6 16.6 7.4c5.1 1 3.5-3.4 3.5-3.4z"/>
            <path class="st182" d="M457.1 1552.9c-.2 6.5 2.5 12.8.5 16.6-.3.6-.9 1.4-1.5 1.7-2.5 1.7-7.5.3-11.6 1.8-.6.2-1-.1-1-.7 0-.9-.2-1.7-.4-2.6-.2-.6-.3-.6-.3.1l.2 3.1c0 .6.6 1.1 1.2 1.1h14.2c.6 0 1.1-.5 1.1-1.1v-20c0-.6-.5-1.1-1.1-1.1h-.2c-.5-.1-1.1.4-1.1 1.1z"/>
            <path class="st181" d="M444.5 1573c4.1-1.5 9.2-.2 11.6-1.8.5-.4 1.2-1.2 1.5-1.7 2-3.8-.7-10.1-.5-16.6 0-.6-.5-1.1-1.1-1.1h-13.4c-.6 0-1.1.5-1.1 1.1l1.1 14.6c0 .6.3 1.6.4 2.2.2.8.4 1.7.4 2.6.1.6.5.9 1.1.7z"/>
            <path class="st182" d="M459.7 1593.6v-15c0-.6-.5-1.1-1.1-1.1-.6 0-1.2.5-1.2 1.1-.1 5.1 2.1 9.9.5 13-.3.6-1 1.4-1.6 1.6-.3.1-.6.3-.9.3h4.3zm-14.6 0c0-.5-.1-.9-.3-1.4-.2-.6-.3-.6-.3.1 0 0 .1.7.1 1.3h.5z"/>
            <path class="st181" d="M455.5 1593.6l.9-.3c.6-.3 1.3-1.1 1.6-1.6 1.6-3-.6-7.9-.5-13 0-.6-.5-1.1-1.1-1.1h-11.7c-.6 0-1.1.5-1.1 1.1l.9 11.3c0 .6.3 1.6.5 2.2.1.5.2.9.3 1.4h10.2z"/>
            <path class="st182" d="M484.8 1554.3c-.8 6.4 1.3 12.5-1 16.2-.3.5-1 1.3-1.6 1.6-2.6 1.6-7.6.3-11.9 1.8-.6.2-.9-.1-.9-.7.1-.8 0-1.6-.2-2.4-.1-.6-.3-.6-.3 0l-.1 3c0 .6.5 1.1 1.1 1.1h14.2c.6 0 1.2-.5 1.3-1.1l1.9-19.5c.1-.6-.4-1.1-1-1.1h-.2c-.6 0-1.2.5-1.3 1.1z"/>
            <path class="st181" d="M470.3 1573.9c4.3-1.5 9.2-.1 11.9-1.8.5-.3 1.2-1.1 1.6-1.6 2.4-3.7.3-9.8 1-16.2.1-.6-.3-1.1-1-1.1h-13.4c-.6 0-1.2.5-1.2 1.1l-.3 14.2c0 .6.1 1.6.3 2.3.2.8.2 1.6.2 2.4 0 .6.3.9.9.7z"/>
            <path class="st182" d="M483.6 1593.6c.3-3.5 1.4-14.2 1.4-14.2.1-.6-.4-1.1-1-1.1s-1.2.5-1.3 1.1c-.6 4.9 1.2 9.7-.7 12.6-.3.5-1.1 1.3-1.7 1.6h3.3zm-14.6 0c0-.3-.1-.6-.1-1-.1-.6-.3-.6-.3 0v.9h.4z"/>
            <path class="st181" d="M480.3 1593.6c.6-.3 1.3-1 1.7-1.6 1.9-2.9.1-7.7.7-12.6.1-.6-.3-1.1-1-1.1H470c-.6 0-1.2.5-1.2 1.1l-.2 11c0 .6.1 1.6.3 2.3.1.3.1.6.1 1h11.3z"/>
          </g>
        </g>
        <text transform="translate(421.988 1618.557)" class="st92 st90 st178">
          Veterans
        </text>
      </g>
      <g id="daytime-icon-3">
        <defs>
          <circle id="SVGID_7_" cx="664.2" cy="1530.5" r="57.1"/>
        </defs>
        <use xlink:href="#SVGID_7_" overflow="visible" opacity=".56" fill="#FFF"/>
        <clipPath id="SVGID_8_">
          <use xlink:href="#SVGID_7_" overflow="visible" opacity=".56"/>
        </clipPath>
        <g class="st187">
          <ellipse class="st188" cx="653.4" cy="1510.6" rx="8.8" ry="9.3"/>
          <ellipse class="st188" cx="648.4" cy="1504.2" rx="4.8" ry="5.1"/>
          <ellipse class="st188" cx="653.1" cy="1502.9" rx="4.8" ry="5.1"/>
          <ellipse class="st188" cx="678.6" cy="1511.4" rx="8.8" ry="9.3"/>
          <ellipse class="st188" cx="679" cy="1504.2" rx="4.8" ry="5.1"/>
          <ellipse class="st188" cx="683.1" cy="1504.5" rx="4.8" ry="5.1"/>
          <ellipse class="st189" cx="666.1" cy="1554.6" rx="21.9" ry="15.3"/>
          <path class="st190" d="M691.7 1587.8c1.1-10.6 2.7-22.6 2.7-27.8 0-10.1-12.8-18.2-28.5-18.2s-28.5 8.1-28.5 18.2c0 5.3 1.6 17.2 2.7 27.8h51.6z"/>
          <path class="st191" d="M666.5 1551.5l-5.4 1.6 3.3 7.7 5.1.1 2.1-8.3z"/>
          <path class="st191" d="M659.1 1587.8c.6-6.4 1.4-12.8 2.2-16.4 1.9-8.5 3.7-11.7 3.7-11.7s3.1-2 4.1.2c1.1 2.3 6.9 8.7 5.6 22.3-.2 1.9-.3 3.8-.4 5.5h-15.2z"/>
          <path class="st11" d="M653.9 1542.7l.6 13.5c.1 1.6 1.3 2.3 2.7 1.5l9.5-5.2 9.2 4.8c1.4.8 2.5.1 2.4-1.6l-1-13.5-9.6-4.3-13.8 4.8z"/>
          <path class="st171" d="M675.8 1544.9c0 8.6-20.2 8.6-20.2 0v-19.6c0-3.9 3.1-7 7-7h6.1c3.9 0 7 3.1 7 7v19.6z"/>
          <path class="st172" d="M646.2 1525.9c.2 1.1 1.3 1.9 2.5 1.7 1.2-.2 2.1-1.2 1.9-2.4l-.9-6.3c-.2-1.1-1.3-1.9-2.5-1.7-1.2.2-2.1 1.2-1.9 2.4l.9 6.3z"/>
          <path class="st173" d="M648.1 1523.3c.1.4.4.7.8.7.4-.1.7-.4.6-.9l-.5-3.7c-.1-.4-.4-.7-.8-.7-.4.1-.7.4-.6.9l.5 3.7z"/>
          <path class="st171" d="M683.6 1526.5c-.2 1.1-1.3 1.9-2.5 1.7-1.2-.2-2.1-1.2-1.9-2.4l.9-6.3c.2-1.1 1.3-1.9 2.5-1.7 1.2.2 2.1 1.2 1.9 2.4l-.9 6.3z"/>
          <path class="st173" d="M681.7 1523.9c-.1.4-.4.7-.8.7-.4-.1-.7-.4-.6-.9l.5-3.7c.1-.4.4-.7.8-.7.4.1.7.4.6.9l-.5 3.7z"/>
          <path class="st172" d="M680.9 1514.5c.7 2.4 0 6 0 8.7 0 11.8-7.1 21.3-15.9 21.3s-15.9-9.5-15.9-21.3c0-4.7-.2-12.4 1.7-15.9 9.7-21.6 30.1-9.6 30.1 7.2z"/>
          <path class="st185" d="M653.8 1519.7c0 .7 1.6.4 3.6.5 2 .1 3.6.5 3.7-.2 0-.7-1.6-1.4-3.6-1.5-2-.1-3.7.5-3.7 1.2z"/>
          <path class="st174" d="M654.5 1519.7c0-.6 1.4-.2 3.1-.2 1.7.1 3.1-.2 3 .4 0 .6-1.4 1-3.1 1-1.7-.1-3-.6-3-1.2z"/>
          <ellipse class="st185" cx="657.3" cy="1519.6" rx="1.1" ry=".9"/>
          <path class="st171" d="M664.3 1512.4c1.5-19.2 16.5-12.4 16.9 2.9 0 2.4-.4 5-.4 7.7 0 11.8-7.1 21.3-15.9 21.3h-.4l-.2-31.9z"/>
          <path class="st185" d="M668.7 1520.3c0 .7 1.6.4 3.6.5 2 .1 3.6.5 3.7-.2 0-.7-1.6-1.4-3.6-1.5-2 0-3.6.5-3.7 1.2z"/>
          <path class="st174" d="M669.4 1520.3c0-.6 1.4-.2 3.1-.2 1.7.1 3.1-.2 3 .4 0 .6-1.4 1-3.1 1-1.7-.1-3-.6-3-1.2z"/>
          <ellipse class="st185" cx="672.2" cy="1520.2" rx="1.1" ry=".9"/>
          <path class="st173" d="M664.9 1544.5c-7.7 0-14.2-7.4-15.6-17.2 1 .9 3.1 2.7 6.4 3.6 2.5.6 4.3-.9 8.4-1.1 3.5-.2 5.7 1.4 8.1.9 4.2-.9 6.3.2 8.3-3.4-1.4 9.8-7.8 17.2-15.6 17.2z"/>
          <path class="st186" d="M664.5 1529.7c3.3-.1 5.4 1.4 7.7.9 4.2-.9 6.9-.8 8.3-3.4-1.4 9.8-7.9 17.3-15.6 17.3h-.4c3.1-1.7 0-14.8 0-14.8z"/>
          <path class="st171" d="M659.9 1534.9c-.1 1.7 2.4.7 4.9.8 2.5.1 4 1.2 4-.5.1-1.7-.4-3-4.3-3.1-3.9-.2-4.5 1.1-4.6 2.8z"/>
          <path class="st175" d="M667.4 1533.6c0-.4-1.4-.2-3.1-.2-1.7 0-3.1-.2-3.2.2 0 .4 1.4.7 3.1.7 1.8 0 3.2-.3 3.2-.7z"/>
          <path class="st172" d="M666.3 1519.6c.5 4.2 2.1 6.5 2.1 8.3 0 1.7-1.8 3-3.1 3s-4.4-1.1-3.7-3.6c.7-2.5 1.8-6.7 1.8-7.6 0-1.8 2.7-1.7 2.9-.1z"/>
          <path class="st171" d="M666.1 1526.2c-1.3-4.3-1.2-7.7-1.2-7.7.9-.3 1.3-.1 1.4.9.5 4.2 2.1 6.8 2.1 8.5 0 1.7-1.8 3-3.1 3-.2 0-.5 0-.8-.1 0-.1 2.8-.4 1.6-4.6z"/>
          <ellipse transform="rotate(-48.187 659.037 1501.66)" class="st192" cx="659" cy="1501.8" rx="4.7" ry="1.8"/>
          <ellipse transform="rotate(-48.226 655.346 1507.48)" class="st192" cx="655.3" cy="1507.5" rx="1.4" ry="1"/>
          <path class="st193" d="M681.4 1518.4v-.5l-4.3-.3c-.7-1.9-2.8-2.5-5.1-2.3-2.3.3-4.7 1.4-5.2 3.4-.3-.5-.7-.9-1.2-1.2-1.3-.7-2.2.4-2.8 2.1-.7-2.2-3.4-2.9-5.9-2.6-2.3.2-4.2 1.3-4.5 3.2l-3.4-3.7-.4.9 3.7 4.1c.3 2.7 2.8 4.7 5.5 4.4 2.6-.3 5.1-2.6 5.2-5.1.5-1.8 1.3-3.2 2.5-2.5.5.3.9.7 1.2 1.4v.2c.3 2.7 3.5 4.7 6.2 4.4 2.7-.3 4.7-2.8 4.4-5.5v-.3l4.1-.1zm-23.7 6.9c-2.4.3-4.5-1.5-4.8-3.8-.3-2.4 1.6-3.4 3.9-3.7 2.4-.3 5.1.3 5.3 2.7.4 2.4-2 4.6-4.4 4.8zm15.3-1.7c-2.4.3-5.2-1.4-5.5-3.8-.3-2.4 2.3-3.5 4.6-3.8 2.4-.3 4.4.4 4.6 2.8.4 2.4-1.4 4.5-3.7 4.8z"/>
          <path class="st194" d="M666.7 1587.8c-.3-7.5-.6-12.7-.7-12.9-1.2-3.3-5.9-9.5-8.1-16.2-2.3-6.7-4.8-13.7-2.7-17.4-4.1.9-20.6 11.5-21 11.9-13.2 10.6.9 7.4 1.8 16.9.5 5.5 1 11.7 1.5 17.6h29.2z"/>
          <path class="st194" d="M664.8 1587.8c.3-7.7.6-13.1.7-13.3 1.2-3.3 5.9-9.5 8.1-16.2 2.3-6.7 4.8-13.7 2.7-17.4 4.1.9 20.6 11.5 21 11.9 13.2 10.6-.9 7.4-1.8 16.9-.5 5.7-1.1 12-1.6 18h-29.1z"/>
          <path class="st195" d="M667.4 1577.5c11.4-10.9 12.5-15.7 12.5-15.7l-3-1.6 3.9-1.1s2.9-6 1.3-11.4c-.6-2.1-.8-2-1.6-3.8 0 0 5.3 4.4 1.9 15.7-3.6 11.2-15 17.9-15 17.9zm-1.6 7.3c-2-9.3-14.2-15.7-14.6-21.3 1.7-.8 3-1.8 3-1.8l-3.9-1.2s-2.9-6.4-1.3-12.2c.6-2.2.9-2.1 1.6-4.1 0 0-5.3 4.7-1.9 16.9 3.6 12.1 11.1 11.8 17.1 23.7z"/>
          <path class="st191" d="M679.8 1574.6h.1l6-6.5 4 7.6"/>
          <path class="st194" d="M717.2 1587.8c-3.9-8.2-13.3-27.9-13.3-27.9-1.8-3.9-6.6-5.4-10.6-3.5-4 1.9-5.8 6.6-3.9 10.4 0 0 5.6 11.8 10 21h17.8zm-83.7 0c4.1-9.3 9.7-21.9 9.7-21.9 1.7-3.9-.2-8.5-4.2-10.3-4.1-1.8-8.8-.1-10.5 3.8 0 0-8.9 20.1-12.6 28.4h17.6z"/>
          <path class="st195" d="M677.887 1577.607l.266-2.888 13.145 1.21-.267 2.89zM669.5 1587.8c-1.7-9.2-4-14.1-4-14.1 1.2 4.6 2.2 9.3 2.9 14.1h1.1z"/>
          <ellipse class="st188" cx="648.4" cy="1509.2" rx="3.1" ry="3.2"/>
          <ellipse class="st188" cx="650.3" cy="1505" rx="3.1" ry="3.2"/>
          <ellipse class="st188" cx="679.1" cy="1505.3" rx="3.1" ry="3.2"/>
          <ellipse class="st188" cx="650.7" cy="1502.2" rx="3.5" ry="3.7"/>
        </g>
        <text transform="translate(593.018 1618.557)" class="st92 st90 st178">
          Faculty &amp; Staff
        </text>
      </g>
    </g>
    <path class="st196" d="M1659.4 103.9c2.4 1.2 4.7 2.5 7 3.8"/>
    <path class="st197" d="M1680.9 115.9c15.9 9.4 31.5 19.3 48.2 28.3l3 3c13 8 25 13 37 22 3 2 6 2 9 4 22 14 43 26 66 39 7 4 13 9 20 13 9.9 5.7 24.7 14.4 37.4 21.8"/>
    <path class="st196" d="M1908.6 251.2c2.5 1.4 4.8 2.8 6.9 4M1 981.6l6.9-4"/>
    <path class="st198" d="M21.7 969.5L1530.3 80"/>
    <path class="st196" d="M1537.2 75.9l6.9-4.1c-.1-.3.3-.4 1-.3l5.8-3.4"/>
    <path class="st199" d="M1566.8 61.9c8.8-1.6 17.2-.3 25.2 2.9"/>
    <path class="st196" d="M1599.7 68.6c.3.2.6.3.9.5l5.2 3c.6-.1.8 0 .7.4l6.9 4.1"/>
    <path class="st200" d="M1626.4 84.4l19.6 11.5"/>
    <path class="st196" d="M1652.5 99.8l6.9 4.1m-255.5 2573c-2.1 1.6-4.6 2.6-7 3.7"/>
    <path class="st201" d="M1383.2 2689c-5.4 3.2-10.8 6.2-16.2 9.2-2 2-4 4-7 5-28 15-53 31-81 48-3 2-6 2-9 4-9 6-17 11-27 16l-3 3c-3 1-6 2-9 4-92 55-176 104-268 158-4 3-8 5-12 8-3 2-5 2-8 4-4 3-8 5-12 8-3 2-6 2-9 4-57 36-110 65-168 100-37 21-48 29.8-85 49.8-7 4-23.5 14.4-30.5 18.4-37.3 22.2-69.4 42.4-105.5 64.2"/>
    <path class="st196" d="M526 3196.7c-2.3 1.4-4.6 2.7-6.9 4.1m935.8-553.9c-2.3 1.4-4.6 2.7-6.9 4.1"/>
    <path class="st202" d="M1435.6 2658.2c-6.2 3.7-12.4 7.3-18.6 11"/>
    <path class="st196" d="M1410.8 2672.8c-.6.4-1.2.7-1.8 1.1l-5.1 3m129.5-1193.3c2.3 1.4 4.6 2.7 6.9 4.1"/>
    <path class="st203" d="M1553.8 1495.9c12.7 7.6 25.5 15.2 39.2 22.4l3 3c13 7 24 13 36 21l12 6c11 8 22 14 34 20l3 3c42 24 80 47 122 72 6 3 11 6 17 9 23 14 44 27 68 40 4.5 3 9 5.8 13.6 8.5"/>
    <path class="st196" d="M1908.4 1704.8c2.3 1.4 4.6 2.7 6.8 4.1M509 1987.5c2.2-1.5 4.5-2.8 6.8-4.2"/>
    <path class="st204" d="M529.6 1975.3c1.5-1 3-2 4.4-3.1 2-1 4-1 5-2 4-3 8-5 12-8 1-1 3-1 5-2 27-18 53-32 81-48 3-2 5-4 8-6 53-31 102-60 155-91 7-5 13-10 21-11 35-21 68-42 104-62 31-18 59-35 90-52 7-4 13-10 20-14 7-3 13-5 20-9 42-26 81-50 123-75 3-1 7-3 10-4l3-3c64-37 122-71 185-110 10-6 21-10 31-16 14-9 29-20 47-18 4 1 9 1 13 3 5 3 10 4 15 7l3 3c12.4 6.7 22.1 14.3 34.2 21.9"/>
    <path class="st196" d="M1526.3 1479.9c2.3 1.2 4.6 2.4 7.1 3.7M4.3 2285.1c2.3-1.3 4.7-2.6 7-3.9"/>
    <path class="st205" d="M25 2273.4c19.2-11.1 38.1-22.6 58-35.1 19-11 37-20 56-31 77-46 150-90 225-136 12.3-5.1 23-12.7 34.5-19.8"/>
    <path class="st196" d="M405.4 2047.5c2.3-1.3 4.7-2.5 7.1-3.7m175.9 1215.7c2.3 1.3 4.6 2.7 6.9 4"/>
    <path class="st206" d="M609.2 3271.5c89.4 51.9 177 104.9 269.8 158.7 38 23 72 43 110 66 29 17 56 33 85 49 4 3 7 5 11 7 18 12 35 21 53 31 202 120 386 229 588 348 11 6 20 12 31 17 4 3 8 5 12 8 1 1 3 1 5 2 11 8 22 14 34 20 15 10 30 18 45 28 3 2 6 2 9 4 15.1 10.6 27.3 15.7 40.7 23.5"/>
    <path class="st196" d="M1909.6 4037.9c2.2 1.4 4.4 2.9 6.6 4.5M0 3506.6c2.4-1.3 4.7-2.6 7-3.9"/>
    <path class="st207" d="M21 3494.7c33.6-19.4 61.5-37 99-59.5 31-18 60-35 91-54 95-56 184-110 278-162 15-5 31-2 44 7 14.2 9.7 27.9 17.2 41.5 25.1"/>
    <path class="st196" d="M581.5 3255.4c2.3 1.3 4.6 2.7 6.9 4.1M509 2048.1c2.3 1.4 4.6 2.7 6.9 4.1"/>
    <path class="st208" d="M529.7 2060.4c16.7 9.9 33.5 19.7 50.3 29.5 23.7 13.8 47.3 27.6 70.9 41.6 11.8 7 23.5 14 35.2 21 5.8 3.5 11.7 7.1 17.5 10.6 5.4 3.3 10.7 7.3 16.5 9.8 12 5.2 22.9 13.5 34.1 20.2 11.5 6.8 22.9 13.7 34.3 20.7 23.2 14.1 46.8 27.6 70.2 41.4 23.7 14 47.4 28 71.1 41.9 23.8 14 47.5 28 71.3 42.1 23.5 13.9 46.9 27.9 70.5 41.5 23.4 13.5 47.1 26.5 70.4 40.2 23.5 13.9 47 28 70.6 41.8 11.5 6.7 23 13.3 34.4 20.1 11.3 6.7 22 14.5 33.4 20.9 2.6 1.5 5.4 2.4 7.9 3.9 2.5 1.6 4.8 3.3 7.2 5 4.9 3.3 10.4 5 15.5 7.9 11.2 6.3 22 13.5 33.1 20.1 23.5 14.1 47.2 27.9 70.9 41.7 23.7 13.9 47.4 27.7 70.9 41.9 11.7 7 23.2 14.3 34.9 21.2 11.6 6.8 23.5 13.1 35 19.9 11.4 6.7 22.6 13.7 33.9 20.5 11.2 6.7 22.9 12.8 34.2 19.4 5.5 3.2 10.4 7.4 16.1 10.2 2.4 1.2 5 2.1 7.3 3.6 2.5 1.6 4.6 3.6 7.1 5.3 5.2 3.5 10.6 6.9 16.1 9.9 5.5 3 11 5.3 16.3 8.7 11 7 22.6 13.1 33.6 20.2 5.1 3.3 10.4 5.5 15.8 8.3 5.4 2.8 10.3 6.6 15.5 9.8 11.5 7 23.1 13.8 34.8 20.5 5.6 3.2 11.3 6.5 17 9.5 5 2.7 9.2 6.3 14.3 8.7 5.6 2.6 10.5 6.2 15.6 9.6 5.4 3.6 11 6.8 16.6 10.1 11.7 6.9 23.3 13.9 34.9 20.7 6.7 3.9 13.4 7.9 20.2 11.7"/>
    <path class="st196" d="M1912 2875.9c2.3 1.3 4.6 2.6 7 3.9M66.2 1786.7c2.3 1.3 4.7 2.6 7 3.9"/>
    <path class="st209" d="M87.2 1798.8c17.2 10.3 34.3 21.1 52.8 30.4 10 6 20 12 31 18 2 1 3 4 5 5 13 7 25 14 38 22 4 2 9 3 13 6 6 4 11 8 17 12 19 11 37 22 56 33 3 2 6 2 9 4 9 5 16 10 25 16 2 1 5 2 7 3 10 5 18 11 28 16 6.4 4.6 13.1 8.6 19.6 12.4"/>
    <path class="st196" d="M395.7 1980.7c2.3 1.4 4.6 2.7 6.9 4.1M1 1748.2c2.3 1.3 4.7 2.6 7 3.9"/>
    <path class="st210" d="M25.1 1762.2c8.5 5.1 17 10.3 25.5 15.5"/>
    <path class="st196" d="M59.2 1782.7c2.3 1.3 4.6 2.7 6.9 4"/>
    <g id="golf-kart-1">
      <path class="st211" d="M1427.7 120.4l-14.5-8.4-5.7 3.3 1.7 1 14.5 8.4 4-2.3 1.7-1z"/>
      <g id="XMLID_14_">
        <path class="st212" d="M1421.1 119.5s.1.1.1.2c-.2 0-.4.1-.7.2l-6.6 3.8-10.1 5.8c-.9.5-1.7 1.9-1.7 2.9v3.7l-.9-.5v-3.7c0-1.1.8-2.4 1.7-2.9l16.7-9.6c.3-.2.5-.2.7-.2.4 0 .6.1.8.3z"/>
        <path class="st159" d="M1420.4 119.1c-.2 0-.5.1-.7.2L1403 129c-.9.5-1.7 1.9-1.7 2.9v3.7l-12.8-7.4v-3.7c0-1.1.8-2.4 1.7-2.9l10.1-5.8 6.6-3.8c.3-.1.5-.2.7-.2l12.8 7.3z"/>
        <path class="st212" d="M1407.5 111.6s.1.1.1.2c-.2 0-.4.1-.7.2l-6.6 3.8-10.1 5.8c-.9.5-1.7 1.9-1.7 2.9v3.7l-.9-.5V124c0-1.1.8-2.4 1.7-2.9l16.7-9.6c.7-.4 1.1-.3 1.5.1z"/>
      </g>
      <g id="XMLID_13_">
        <path class="st159" d="M1398.6 100.7v16.1l-1 .5v-16.1z"/>
        <path class="st213" d="M1398.6 100.7l-1 .5-.8-.4.9-.6zm-1 .5v16.1l-.8-.4v-16.1z"/>
      </g>
      <g id="XMLID_12_">
        <path class="st159" d="M1363.9 144.5c0 2.2-1.5 4.8-3.4 5.9-1 .6-1.8.6-2.5.2-.6-.4-.9-1.1-.9-2.2 0-2.2 1.5-4.8 3.4-5.9.9-.5 1.8-.6 2.4-.3.6.5 1 1.2 1 2.3zm-3.4 4.5c1.2-.7 2.1-2.3 2.1-3.7 0-.9-.4-1.5-1.1-1.5-.3 0-.7.1-1 .3-1.2.7-2.1 2.3-2.1 3.7 0 .4.1.8.3 1 .3.5 1 .6 1.8.2z"/>
        <path class="st214" d="M1360.3 140.9l2.6 1.5c-.6-.3-1.5-.3-2.4.3-1.9 1.1-3.4 3.7-3.4 5.9 0 1.1.4 1.8.9 2.2l-2.6-1.5c-.6-.4-.9-1.1-.9-2.2 0-2.2 1.5-4.8 3.4-5.9 1-.6 1.8-.7 2.4-.3z"/>
        <path class="st214" d="M1362.6 145.3c0 1.3-1 3-2.1 3.7-.8.5-1.5.4-1.9-.2.3 0 .7-.1 1-.3 1.2-.7 2.1-2.3 2.1-3.7 0-.4-.1-.8-.3-1 .8 0 1.2.6 1.2 1.5z"/>
        <path class="st92" d="M1361.5 143.8c.2.3.3.6.3 1 0 1.3-1 3-2.1 3.7-.4.2-.7.3-1 .3-.2-.2-.3-.6-.3-1 0-1.3 1-3 2.1-3.7.4-.2.7-.3 1-.3z"/>
      </g>
      <g id="XMLID_10_">
        <path class="st215" d="M1413.6 108.7l.8 5-.7.5-.8-5c-.2-1.1-.8-1.8-1.6-2-.5-.1-1 0-1.5.3l-2.6 1.5v1.6c0 .6-.4 1.4-1 1.7l-3.9 2.3c-.3.2-.5.2-.7.1l-.1-.1c-.1-.2-.2-.4-.1-.8.5-1.9 2.4-4.2 4.8-5.7.3-.2.5-.2.7-.1h.1l.2.2 2.6-1.6c.7-.4 1.4-.5 1.9-.3.1 0 .3.1.4.2l.1.1c.8.4 1.2 1.2 1.4 2.1zm-7 2.3v-2c0-.2-.1-.3-.3-.2-.2.1-.4.2-.5.4-1.4 1-2.6 2.3-3.2 3.5-.2.3-.3.7-.4 1v.1h.2l3.9-2.3c.2 0 .3-.3.3-.5z"/>
        <path class="st216" d="M1412.9 109.3l.8 5-.9-.5-.8-5c-.1-.6-.4-1.2-.7-1.5.8.1 1.4.9 1.6 2z"/>
        <path class="st217" d="M1411.5 106.2l.7.4c-.1-.1-.2-.1-.4-.2-.6-.2-1.3-.1-1.9.3l-2.6 1.6c0-.1-.1-.2-.2-.2h-.1l-.5-.3 2.5-1.5c.8-.5 1.7-.5 2.4-.1h.1z"/>
        <path class="st218" d="M1406.2 107.6l.3.2.5.3c-.2-.1-.4-.1-.7.1-2.3 1.5-4.2 3.8-4.8 5.7-.1.3-.1.6.1.8l.1.1-.8-.5s-.1 0-.1-.1c-.1-.2-.2-.4-.1-.8.5-1.9 2.4-4.2 4.8-5.7.2-.2.5-.3.7-.1z"/>
        <path class="st214" d="M1406.6 109.1v2c0 .2-.1.5-.3.6l-3.9 2.3c-.1.1-.2 0-.2 0v-.1c.1-.3.2-.7.4-1l2.9-1.7c.2-.1.3-.4.3-.6v-1.3c.2-.1.4-.3.5-.4.2-.1.3 0 .3.2z"/>
      </g>
      <g id="XMLID_9_">
        <path class="st219" d="M1420.7 117.4v.8c0 .3-.2.7-.5.9l-6.8 3.9c-.2.1-.3.1-.4 0-.1-.1-.1-.2-.1-.3v-.8c0-.3.2-.7.5-.9l6.8-3.9c.1-.1.3-.1.3 0 .2 0 .2.1.2.3z"/>
        <path class="st220" d="M1420.6 117c-.1 0-.2 0-.4.1l-6.8 3.9c-.3.2-.5.6-.5.9v.8c0 .1 0 .2.1.3l-2.2-1.3.1-.3c.1 0 .2.1.3.1v-.5c-.1 0-.2-.1-.2-.2l-.5-2.2 2.4 1.4.1.1c.1 0 .2 0 .3-.1l.5-.5c.2-.2.4-.5.3-.8l-.9-3.5h.1c.3-.2.5-.6.5-.9v-.4l.3-.2c.1-.1.3-.1.4 0l6.1 3.3z"/>
        <path class="st219" d="M1414.2 118.7c.1.2-.1.6-.3.8l-.5.5c-.1.1-.2.1-.3.1l-.1-.1s0-.1-.1-.1l-1-3.9 1.5-.8.8 3.5z"/>
        <path class="st220" d="M1413.9 113.9v.4c0 .3-.2.7-.5.9h-.1l-.2-.8.8-.5z"/>
        <path class="st221" d="M1413.9 113.5v.4l-.8.5-.2-.9.5-.3c.1-.1.3-.1.3 0 .1 0 .2.1.2.3z"/>
        <path class="st220" d="M1413.8 113.1c-.1 0-.2 0-.4.1l-.5.3-.1-.2c0-.1 0-.1-.1-.1l-.1-.1-5.5-3.2.3-.2c.1-.1.3-.1.4 0l6 3.4z"/>
        <path class="st219" d="M1413.1 114.3l.2.9-1.4.8-.2-.8z"/>
        <path class="st219" d="M1412.9 113.5l.2.9-1.5.8-.2-.7v-.2l1.5-.8z"/>
        <path class="st222" d="M1412.9 120l-2.4-1.4-.1-.4c-.1-.3 0-.7.2-1.1l.1-.1-.1-.3 1.3-.7 1 3.9v.1z"/>
        <path class="st219" d="M1412.8 113.3l.1.2-1.4.8c0-.2.1-.4.3-.6l.5-.5c.1-.1.3-.2.4-.1l.1.1v.1z"/>
        <path class="st222" d="M1407.2 109.9l5.5 3.2c-.1 0-.2 0-.4.1l-.5.5c-.2.2-.3.4-.3.6l-3.6 2.1c0-.2.1-.5.2-.7l.1-.1-.1-.4-.2.4c-.2.3-.3.7-.3 1l-.3.2-.3-.2s0-.1-.1-.1l-.2-.6.4-.3c.2-.2.4-.5.3-.8l-1.1-4.4.9-.5zm4.5 5.3l.2.8-1.3.7-.1.1-1.6.9-.8-.5z"/>
        <path class="st222" d="M1411.7 115.2l-3.6 2.1-.1-.1-.1-.4v-.4l3.6-2.1v.2l.2.7z"/>
        <path class="st92" d="M1411.2 121.1v.5c-.1 0-.2 0-.3-.1-.1-.1-.2-.2-.2-.3l-.6-2.6v-.1l.4.3.5 2.2s.1 0 .2.1z"/>
        <path class="st220" d="M1410.9 121.5l-.1.3-3.7-2.1c-.1 0-.2-.2-.2-.3v-.4l.9-.5.3 1.3c.1.3.3.4.5.4v-.5c-.1 0-.2-.1-.2-.2l-.3-1.2.8-.4 1.1.6v.1l.6 2.6.3.3z"/>
        <path class="st92" d="M1410.6 116.7l.1.3-.1.1c-.2.3-.3.8-.2 1.1l.1.4-.4-.3c0-.4.1-.9.3-1.3l.1-.2.1-.1zm0 0l-.1.1z"/>
        <path class="st222" d="M1410.5 116.8l-.1.2c-.2.4-.4.9-.3 1.3l-1.1-.6 1.5-.9z"/>
        <path class="st220" d="M1408.9 117.7l-.7.5-.2-.9.1-.1z"/>
        <path class="st92" d="M1408.7 119.6v.5c-.3 0-.5-.1-.5-.4l-.3-1.3.4-.2.3 1.2c-.1.1 0 .2.1.2zm-.7-2.3l.2.9-.4.2-.2-.9zm0-2.1l.1.4-.1.1c-.1.2-.2.5-.2.7l-.3.2c0-.3.1-.7.3-1l.2-.4z"/>
        <path class="st222" d="M1408.1 117.2l-.1.1v-.2z"/>
        <path class="st92" d="M1408 117.1v.1l-.4.2-.1-.5v-.1l.5.3z"/>
        <path class="st92" d="M1407.9 116.7l.1.4-.4-.3v-.3l.3-.2c-.1.2-.1.3 0 .4z"/>
        <path class="st220" d="M1407.6 117.5l.2.9-.9.5v-.4c0-.3.2-.7.5-.9l.2-.1z"/>
        <path class="st221" d="M1407.5 117l.1.5-.2.1c-.3.2-.5.6-.5.9v.4l-.3.2c-.2.1-.3.1-.4 0-.1-.1-.1-.2-.1-.3v-.8c0-.3.2-.7.5-.9l.6-.4.3.1v.2z"/>
        <path class="st222" d="M1407.2 116.7l.3-.2v.3l-.3-.1zm.2-1.9c.1.2-.1.6-.3.8l-.4.3-1.2-4.8v-.2l.8-.5 1.1 4.4z"/>
        <path class="st220" d="M1407.2 116.7l-.6.4c-.3.2-.5.6-.5.9v.8c0 .1 0 .2.1.3l-2.2-1.3.1-.3c.1 0 .2.1.3.1v-.5c-.1 0-.2-.1-.2-.2l-.5-2.2 2.4 1.4.1.1c.1 0 .2 0 .3-.1l.2-.2.2.6s0 .1.1.1l.2.1z"/>
        <path class="st222" d="M1406.8 109.7l.3.2-.9.5-.1-.5.2-.2c.2 0 .3-.1.5 0z"/>
        <path class="st219" d="M1405.5 111l1.2 4.8-.2.2c-.1.1-.2.1-.3.1l-.1-.1s0-.1-.1-.1l-1.2-4.7.7-.4v.2z"/>
        <path class="st222" d="M1406.2 109.9l.1.5-.8.5c0-.2.1-.4.3-.6l.4-.4z"/>
        <path class="st219" d="M1406 109.3l.2.6-.4.3c-.2.2-.3.4-.3.6l-.7.4-.2-.7c-.1-.2.1-.6.3-.8l.5-.5c.1-.1.3-.2.4-.1l.1.1c.1 0 .1.1.1.1z"/>
        <path class="st222" d="M1406.1 116.1l-2.4-1.4-.1-.4c-.1-.3 0-.7.2-1.1l.1-.1-.1-.4-.2.4c-.2.4-.4.9-.3 1.3l-2-1.1 3.6-2.1 1.2 4.7v.2z"/>
        <path class="st222" d="M1400 105.8l5.9 3.4c-.1 0-.2 0-.4.1l-.5.5c-.2.2-.4.5-.3.8l.2.7-3.6 2.1-.1-.1-.1-.4c-.1-.3 0-.7.2-1.1l.1-.1-.1-.4-.2.4c-.2.4-.4.9-.3 1.3l-.5-.3s0-.1-.1-.1l-1.4-5.4c-.1-.2.1-.6.3-.8l.5-.5c.1-.2.2-.2.4-.1z"/>
        <path class="st92" d="M1404.4 117.1v.5c-.1 0-.2 0-.3-.1-.1-.1-.2-.2-.2-.3l-.6-2.6v-.1l.4.3.5 2.2s.1.1.2.1z"/>
        <path class="st220" d="M1404.1 117.5l-.1.3-3.7-2.1c-.1 0-.2-.2-.2-.3v-.8c0-.3.2-.7.5-.9l.2-.1.5 2.2c.1.3.3.4.5.4v-.5c-.1 0-.2-.1-.2-.2l-.5-2.1.1-.1 2 1.1v.1l.6 2.6c.1.3.2.4.3.4z"/>
        <path class="st92" d="M1403.8 112.7l.1.4-.1.1c-.2.3-.3.8-.2 1.1l.1.4-.4-.3c0-.4.1-.9.3-1.3l.2-.4zm-2 3v.5c-.3 0-.5-.1-.5-.4l-.5-2.2.4-.2.5 2.1c0 .1 0 .1.1.2zm-.6-4.5l.1.4-.1.1c-.2.3-.3.8-.2 1.1l.1.4-.4-.3c0-.4.1-.9.3-1.3l.2-.4zm-.1 2v.1l-.4.2-.1-.5v-.1l.5.3z"/>
      </g>
      <path class="st217" d="M1421.4 119.6c.2 0 .4.1.6.3l-6.3 3.7c-2.6 1.5-4.9 4.8-5.6 8l-7.9 4.5v-3.7c0-1.1.8-2.4 1.7-2.9l10.1-5.8 6.6-3.8c.3-.1.5-.2.7-.2 0-.1.1-.1.1-.1z"/>
      <path class="st212" d="M1422.8 120.5l-6.3 3.7c-2.6 1.5-4.9 4.8-5.6 8l-.9-.5c.7-3.2 3-6.5 5.6-8l6.3-3.7.9.5z"/>
      <path class="st214" d="M1420.7 126.4c.2.5.3 1.1.3 1.8l-1.7-1c0-.9-.2-1.7-.6-2.3.9.1 1.6.6 2 1.5z"/>
      <path class="st214" d="M1421.1 128.2c0-.7-.1-1.3-.3-1.8l1.3-.7 1.7-1 4-2.3 1.7-1v2l-5.7 3.3-2.7 1.5z"/>
      <path class="st92" d="M1419.4 127.2l-7.2 4.1c.7-2.3 2.3-4.7 4.3-5.8.8-.5 1.6-.7 2.3-.6.3.6.6 1.4.6 2.3zm-48.5 21.8c0 .2.1.4.2.5h.1l1.6.9h.1c.1.1.3 0 .6-.1l1.5-.9c.8-.5 1.6-.7 2.3-.6.4.5.6 1.3.6 2.3l-7.7 2.5c-.9.3-1.4-.4-1-1.6l.6-2c.1-.4.4-.8.6-.9.3 0 .5-.1.5-.1z"/>
      <path class="st212" d="M1410.9 132.1l-21.4 12.4-5.3 3.1c-.9.5-2.1.5-2.6-.1l-.4-.5c.4 0 .9-.1 1.3-.4l18.8-11 .9.5 7.9-4.5.8.5z"/>
      <path class="st214" d="M1377.3 149c1.4.1 2.3 1.3 2.3 3.2l-1.7-1c0-.9-.2-1.7-.6-2.2z"/>
      <g id="XMLID_7_">
        <path class="st159" d="M1420.7 129.4c0 2.2-1.5 4.8-3.4 5.9-1 .6-1.8.6-2.5.2-.6-.4-.9-1.1-.9-2.2 0-2.2 1.5-4.8 3.4-5.9.9-.5 1.8-.6 2.4-.3.6.4 1 1.2 1 2.3zm-3.4 4.4c1.2-.7 2.1-2.3 2.1-3.7 0-.9-.4-1.5-1.1-1.5-.3 0-.7.1-1 .3-1.2.7-2.1 2.3-2.1 3.7 0 .4.1.8.3 1 .3.5 1 .7 1.8.2z"/>
        <path class="st214" d="M1412.3 134c-.6-.4-.9-1.1-.9-2.2 0-2.2 1.5-4.8 3.4-5.9.9-.5 1.8-.6 2.4-.3l2.6 1.5c-.6-.3-1.5-.3-2.4.3-1.9 1.1-3.4 3.7-3.4 5.9 0 1.1.4 1.8.9 2.2l-2.6-1.5z"/>
        <path class="st218" d="M1419.4 130.1c0 1.3-1 3-2.1 3.7-.8.5-1.5.4-1.9-.2.3 0 .7-.1 1-.3 1.2-.7 2.1-2.3 2.1-3.7 0-.4-.1-.8-.3-1 .8 0 1.2.6 1.2 1.5z"/>
        <path class="st223" d="M1418.3 128.6c.2.3.3.6.3 1 0 1.3-1 3-2.1 3.7-.4.2-.7.3-1 .3-.2-.2-.3-.6-.3-1 0-1.3 1-3 2.1-3.7.4-.2.7-.3 1-.3z"/>
      </g>
      <g id="XMLID_6_">
        <path class="st159" d="M1379.2 153.4c0 2.2-1.5 4.8-3.4 5.9-1 .6-1.8.6-2.5.2-.6-.4-.9-1.1-.9-2.2 0-2.2 1.5-4.8 3.4-5.9.9-.5 1.8-.6 2.4-.3.6.4 1 1.2 1 2.3zm-3.4 4.4c1.2-.7 2.1-2.3 2.1-3.7 0-.9-.4-1.5-1.1-1.5-.3 0-.7.1-1 .3-1.2.7-2.1 2.3-2.1 3.7 0 .4.1.8.3 1 .3.6 1 .7 1.8.2z"/>
        <path class="st214" d="M1370.8 158c-.6-.4-.9-1.1-.9-2.2 0-2.2 1.5-4.8 3.4-5.9.9-.5 1.8-.6 2.4-.3l2.6 1.5c-.6-.3-1.5-.3-2.4.3-1.9 1.1-3.4 3.7-3.4 5.9 0 1.1.4 1.8.9 2.2l-2.6-1.5z"/>
        <path class="st218" d="M1378 154.1c0 1.3-1 3-2.1 3.7-.8.5-1.5.4-1.9-.2.3 0 .7-.1 1-.3 1.2-.7 2.1-2.3 2.1-3.7 0-.4-.1-.8-.3-1 .7.1 1.2.6 1.2 1.5z"/>
        <path class="st223" d="M1376.9 152.6c.2.3.3.6.3 1 0 1.3-1 3-2.1 3.7-.4.2-.7.3-1 .3-.2-.2-.3-.6-.3-1 0-1.3 1-3 2.1-3.7.3-.2.7-.3 1-.3z"/>
      </g>
      <path class="st224" d="M1422.8 120.5c.5.5.7 1.4.8 2.3.1 1 .1 1.9.1 1.9l-1.7 1-1.3.7c-.4-.9-1.1-1.4-2-1.5-.7-.1-1.5.1-2.3.6-1.9 1.1-3.6 3.4-4.3 5.8-.2.7-.3 1.5-.3 2.2l-32.3 18.7c0-2-.9-3.1-2.3-3.2-.7-.1-1.5.1-2.3.6l-1.5.9c-.2.1-.4.1-.6.1h-.1c-.1-.1-.2-.3-.2-.5v-1.4s1.5-.9 3.3-1.9c1.8-1.1 3.3-1.9 3.3-1.9l1.9 2.2.4.5c.5.6 1.7.7 2.6.1l5.3-3.1 21.4-12.4c.7-3.2 3-6.5 5.6-8l6.5-3.7z"/>
      <g id="XMLID_5_">
        <path class="st223" d="M1420.9 116.9v1.6c0 .6-.4 1.4-1 1.7l-3.9 2.3c-.3.2-.5.2-.7.1l-.1-.1c-.1-.2-.2-.4-.1-.8.5-1.9 2.4-4.2 4.8-5.7.3-.2.5-.2.7-.1h.1l.2.2m-.6 2.8v-2c0-.2-.1-.3-.3-.2-.2.1-.4.2-.5.4-1.4 1-2.6 2.3-3.2 3.5-.2.3-.3.7-.4 1v.1h.2l3.9-2.3c.1 0 .3-.3.3-.5z"/>
        <path class="st218" d="M1419.8 115.5l.3.2.5.3c-.2-.1-.4-.1-.7.1-2.3 1.5-4.2 3.8-4.8 5.7-.1.3-.1.6.1.8l.1.1-.8-.5s-.1 0-.1-.1c-.1-.2-.2-.4-.1-.8.5-1.9 2.4-4.2 4.8-5.7.3-.3.5-.3.7-.1z"/>
        <path class="st214" d="M1420.3 116.9v2c0 .2-.1.5-.3.6l-3.9 2.3c-.1.1-.2 0-.2 0v-.1c.1-.3.2-.7.4-1l2.9-1.7c.2-.1.3-.4.3-.6v-1.3c.2-.1.4-.3.5-.4.1-.1.3 0 .3.2z"/>
      </g>
      <path class="st212" d="M1374.6 136.4l-1.7-1 14.8-7.6.8.5-14.6 7.7 1.1.2z"/>
      <path class="st223" d="M1378.6 138.7l-.1-.1-4.5-2.6 14.6-7.7 12.8 7.4-18.8 11c-.4.2-.9.4-1.3.4l-1.5-1.8-.9-6.1c-.1-.3-.2-.4-.3-.5z"/>
      <path class="st214" d="M1378.8 139.1l.9 6.1-.4-.5-.8-4.5-1.7-1 1-.6c.2-.1.4-.2.6-.1l.1.1c.2.2.3.3.3.5z"/>
      <path class="st159" d="M1365.8 131.3l12.6 7.3c-.2-.1-.4 0-.6.1l-1 .6-10.6-6.1-2.2-1.3 1-.6c.2-.1.4-.2.6-.1l.2.1z"/>
      <g id="XMLID_4_">
        <path class="st217" d="M1412.2 108.6v16.1l-.9.5v-16.1z"/>
        <path class="st213" d="M1412.2 108.6l-.9.5-.9-.5.9-.5z"/>
        <path class="st213" d="M1411.3 109.1v16.1l-.9-.5v-16.1z"/>
      </g>
      <path class="st224" d="M1378.5 140.2l.8 4.5s-1.5.9-3.3 1.9c-1.8 1.1-3.3 1.9-3.3 1.9s.5-2.6 1.5-4.1c1.7-2.4 4.3-4.2 4.3-4.2z"/>
      <path class="st225" d="M1363.1 144.5l-4.2-2.4-.8-.5s-.1.1-.3.2h-.1c-.2.1-.5.5-.6.9l-.6 2c-.3.8-.1 1.4.3 1.6l12.7 7.3c-.3-.3-.4-.8-.1-1.5l.6-2c.1-.4.4-.8.6-.9l.4-.2-7.9-4.5z"/>
      <path class="st159" d="M1358.1 140.2v1.4s-.1.1-.3.2l-1.1-.6c-.2-.1-.3-.3-.3-.6v-1.4s.5-2.6 1.5-4.1c1.7-2.4 4.4-4.2 4.4-4.2l1.7 1 12.8 7.4 1.7 1s-2.6 1.8-4.4 4.2c-1.1 1.5-1.5 4.1-1.5 4.1v1.4c0 .2.1.4.2.5l-1.6-.9h-.1c-.1-.1-.2-.3-.2-.5v-1.4l-12.8-7.5z"/>
      <path class="st214" d="M1358.1 141.6v-1.4l12.8 7.4v1.4l-7.8-4.5z"/>
      <path class="st212" d="M1380.5 126.2l-4.7 2.6c-.9.5-1.7 1.9-1.7 2.9v3.7l.9.5v-3.7c0-1.1.8-2.4 1.7-2.9l5.7-2.9c-.3-.2-.9-.6-1.9-.2z"/>
      <path class="st159" d="M1381 126.9l-4.4 2.5c-.9.5-1.7 1.9-1.7 2.9v3.7l8.7-4.9c0-6.4-2-4.5-2.6-4.2z"/>
      <path class="st159" d="M1395.2 133.9l-12.7-7.4-5.8 2.9c-.9.5-1.7 1.9-1.7 2.9v3.7l12.8 7.4v-3.7c0-1.1.8-2.4 1.7-2.9l5.7-2.9z"/>
      <path class="st212" d="M1379.7 126.6l-3.9 2.3c-.9.5-1.7 1.9-1.7 2.9v3.7l.9.5v-3.7c0-1.1.8-2.4 1.7-2.9l5.2-3c-.8.2-1.5.5-2.2.2zm14.4 7.4l-4.7 2.7c-.9.5-1.7 1.9-1.7 2.9v3.7l.9.5v-3.7c0-1.1.8-2.4 1.7-2.9l5.9-2.9c-.3-.1-1.1-.6-2.1-.3z"/>
      <path class="st217" d="M1394.6 134.7l-4.4 2.5c-.9.5-1.7 1.9-1.7 2.9v3.7l8.7-4.9c0-6.3-2-4.4-2.6-4.2z"/>
      <g id="XMLID_18_">
        <path class="st159" d="M1397.2 113.8v2.6c0 .8-.6 1.8-1.3 2.2l-5.1 3c-.3.2-.6.2-.8.1h-.1s-.1 0-.1-.1c-.2-.2-.2-.6-.1-1 .7-2.4 3.2-5.4 6.2-7.4.3-.2.7-.3.9-.2h.1c.1.1.3.4.3.8zm-.9 3.1v-2.6c0-.3-.2-.4-.4-.2-.2.1-.3.2-.5.3-2.1 1.5-3.9 3.5-4.7 5.2-.1.3-.3.6-.3.9v.1s.1.1.3 0l5.1-3c.3-.1.5-.5.5-.7z"/>
        <path class="st218" d="M1396 112.5l.8.4c-.2-.1-.6-.1-.9.2-3 2-5.5 5-6.2 7.4-.1.4-.1.8.1 1l.1.1-.8-.4h-.1s-.1 0-.1-.1c-.2-.2-.2-.6-.1-1 .7-2.4 3.1-5.4 6.2-7.4.4-.3.7-.3 1-.2z"/>
        <path class="st214" d="M1396.3 115.9v1c0 .3-.2.6-.4.7l-5.1 3c-.1.1-.2.1-.3 0v-.1l.3-.9 4.2-2.4c.2-.1.4-.5.4-.7v-2c.2-.1.3-.2.5-.3.2-.1.4 0 .4.2v1.5z"/>
      </g>
      <g id="XMLID_17_">
        <path class="st219" d="M1410.8 114.6c.1.1.2.2.1.4l-1 5.1c-.1.3-.3.6-.5.6l-.5.1h-.3c-.1-.1-.1-.2-.1-.4l1-5.1c.1-.3.3-.6.5-.6l.5-.2c.2.1.2.1.3.1z"/>
        <path class="st226" d="M1410.8 114.6h-.2l-.5.2c-.2.1-.5.4-.5.6l-1 5.1c0 .2 0 .3.1.4l-.2-.1-2.1-1.2-.4-.2-3.2-1.8c-.1-.1-.1-.2-.1-.4v-.2c.2-.1.4-.4.5-.6l.9-4.9.5-.2h.2l6 3.3z"/>
        <path class="st219" d="M1409.1 124.3v.8c0 .3-.2.7-.5.9l-6.8 3.9c-.2.1-.3.1-.4 0-.1-.1-.1-.2-.1-.3v-.8c0-.3.2-.7.5-.9l6.8-3.9c.1-.1.3-.1.3 0 .1 0 .2.2.2.3z"/>
        <path class="st226" d="M1408.9 124c-.1 0-.2 0-.4.1l-6.8 3.9c-.3.2-.5.6-.5.9v.8c0 .1 0 .2.1.3l-5.9-3.4c-.1 0-.2-.2-.2-.3v-.4l6.4-3.7c.3-.2.5-.6.5-.9v-.4l.3-.2c.1-.1.2-.1.3-.1h.1l2.1 1.2.4.2 2.2 1.3.4.2 1 .5z"/>
        <path class="st92" d="M1408.9 120.9l-.2 1.1c-.1.5-.3 1-.7 1.4l-.4-.2c.3-.3.5-.7.5-1l.3-1.4.2.1c.1.1.2.1.3 0zm-2.6-1.3l-.2 1c-.1.5-.3 1-.7 1.4l-.4-.2c.3-.3.5-.7.5-1l.3-1.4.5.2z"/>
        <path class="st222" d="M1404 110.7c.1.1.2.2.1.4v.2c-.2.1-.4.4-.5.6l-.9 4.9-.5.1h-.3c-.1-.1-.1-.2-.1-.4l1-5.1c.1-.3.3-.6.5-.6l.5-.2c.1.1.1.1.2.1z"/>
        <path class="st226" d="M1404.1 111.4l-.9 4.9c-.1.3-.3.5-.5.6l.9-4.9c0-.3.2-.5.5-.6z"/>
        <path class="st226" d="M1404 110.7h-.2l-.5.2c-.2.1-.5.4-.5.6l-1 5.1c0 .2 0 .3.1.4l-.2-.1-2.1-1.2-.4-.2-3.2-1.8c-.1-.1-.1-.2-.1-.4l1-5.1c.1-.3.3-.6.5-.6l.5-.2h.2l5.9 3.3zm-1.7 10.1v.4c0 .3-.2.7-.5.9l-6.4 3.7v-.4c0-.3.2-.7.5-.9l6.4-3.7z"/>
        <path class="st222" d="M1402.3 120.4v.4l-6.5 3.7c-.3.2-.5.6-.5.9v.4l-.3.2c-.2.1-.3.1-.4 0-.1-.1-.1-.2-.1-.3v-.8c0-.3.2-.7.5-.9l6.8-3.9c.1-.1.3-.1.3 0 .1 0 .2.1.2.3z"/>
        <path class="st226" d="M1402.1 120c-.1 0-.2 0-.4.1l-6.8 3.9c-.3.2-.5.6-.5.9v.8c0 .1 0 .3.1.3l-5.9-3.4c-.1 0-.2-.2-.2-.3v-.8c0-.3.2-.7.5-.9l6.8-3.9c.1-.1.2-.1.3-.1h.1l2.1 1.2.4.2 2.2 1.3.4.2.9.5z"/>
        <path class="st92" d="M1402.1 117l-.2 1.1c-.1.5-.3 1-.7 1.4l-.4-.2c.3-.3.5-.7.5-1l.3-1.4.2.1h.3zm-2.6-1.3l-.2 1c-.1.5-.3 1-.7 1.4l-.4-.2c.3-.3.5-.7.5-1l.3-1.4.5.2z"/>
      </g>
      <g id="XMLID_1_">
        <path class="st223" d="M1410.8 121.7v2.6c0 .8-.6 1.8-1.3 2.2l-5.1 3c-.3.2-.6.2-.8.1h-.1s-.1 0-.1-.1c-.2-.2-.2-.6-.1-1 .7-2.4 3.2-5.4 6.2-7.4.3-.2.7-.3.9-.2h.1c.2.1.3.4.3.8zm-.9 3v-2.6c0-.3-.2-.4-.4-.2-.2.1-.3.2-.5.3-2.1 1.5-3.9 3.5-4.7 5.2-.1.3-.3.6-.3.9v.1s.1.1.3 0l5.1-3c.3-.1.5-.4.5-.7z"/>
        <path class="st218" d="M1409.6 120.4l.8.4c-.2-.1-.6-.1-.9.2-3 2-5.5 5-6.2 7.4-.1.4-.1.8.1 1l.1.1-.8-.4h-.1s-.1 0-.1-.1c-.2-.2-.2-.6-.1-1 .7-2.4 3.1-5.4 6.2-7.4.4-.4.8-.4 1-.2z"/>
        <path class="st214" d="M1409.9 123.7v1c0 .3-.2.6-.4.7l-5.1 3c-.1.1-.2.1-.3 0v-.1l.3-.9 4.2-2.4c.2-.1.4-.5.4-.7v-2c.2-.1.3-.2.5-.3.2-.1.4 0 .4.2v1.5z"/>
      </g>
      <g id="XMLID_11_">
        <path class="st159" d="M1381.8 122.6v2.6c0 .8-.6 1.8-1.3 2.2l-5.1 3c-.3.2-.6.2-.8.1h-.1s-.1 0-.1-.1c-.2-.2-.2-.6-.1-1 .7-2.4 3.1-5.4 6.2-7.4.3-.2.7-.3.9-.2h.1c.2.1.3.4.3.8zm-.9 3V123c0-.3-.2-.4-.4-.2-.2.1-.3.2-.5.3-2.1 1.5-3.9 3.5-4.7 5.2-.1.3-.3.6-.3.9v.1s.1.1.3 0l5.1-3c.3-.1.5-.4.5-.7z"/>
        <path class="st218" d="M1380.6 121.3l.8.4c-.2-.1-.6-.1-.9.2-3 2-5.5 5-6.2 7.4-.1.4-.1.8.1 1l.1.1-.8-.4h-.1s-.1 0-.1-.1c-.2-.2-.2-.6-.1-1 .7-2.4 3.1-5.4 6.2-7.4.4-.4.8-.4 1-.2z"/>
        <path class="st214" d="M1380.9 124.6v1c0 .3-.2.6-.4.7l-5.1 3c-.1.1-.2.1-.3 0v-.1l.3-.9 4.2-2.4c.2-.1.4-.5.4-.7v-2c.2-.1.3-.2.5-.3.2-.1.4 0 .4.2v1.5z"/>
      </g>
      <g id="XMLID_8_">
        <path class="st219" d="M1395.4 123.4c.1.1.2.2.1.4l-1 5.1c-.1.3-.3.6-.5.6l-.5.1h-.3c-.1-.1-.1-.2-.1-.4l1-5.1c.1-.3.3-.6.5-.6l.5-.2c.2.1.3.1.3.1z"/>
        <path class="st227" d="M1395.4 123.4h-.2l-.5.2c-.2.1-.5.4-.5.6l-1 5.1c0 .2 0 .3.1.4l-.2-.1-2.1-1.2-.4-.2-3.2-1.8c-.1-.1-.1-.2-.1-.4v-.2c.2-.1.4-.4.5-.6l.9-4.9.5-.2h.2l6 3.3z"/>
        <path class="st219" d="M1393.7 133.1v.8c0 .3-.2.7-.5.9l-6.8 3.9c-.2.1-.3.1-.4 0-.1-.1-.1-.2-.1-.3v-.8c0-.3.2-.7.5-.9l6.8-3.9c.1-.1.3-.1.3 0 .2 0 .2.1.2.3z"/>
        <path class="st226" d="M1393.6 132.7c-.1 0-.2 0-.4.1l-6.8 3.9c-.3.2-.5.6-.5.9v.8c0 .1 0 .2.1.3l-5.9-3.4c-.1 0-.2-.2-.2-.3v-.4l6.4-3.7c.3-.2.5-.6.5-.9v-.4l.3-.2c.1-.1.2-.1.3-.1h.1l2.1 1.2.4.2 2.2 1.3.4.2 1 .5z"/>
        <path class="st92" d="M1393.5 129.7l-.2 1.1c-.1.5-.3 1-.7 1.4l-.4-.2c.3-.3.5-.7.5-1l.3-1.4.2.1h.3zm-2.5-1.3l-.2 1c-.1.5-.3 1-.7 1.4l-.4-.2c.3-.3.5-.7.5-1l.3-1.4.5.2z"/>
        <path class="st222" d="M1388.6 119.5c.1.1.2.2.1.4v.2c-.2.1-.4.4-.5.6l-.9 4.9-.5.1h-.3c-.1-.1-.1-.2-.1-.4l1-5.1c.1-.3.3-.6.5-.6l.5-.2c.1.1.2.1.2.1z"/>
        <path class="st226" d="M1388.7 120.1l-.9 4.9c-.1.3-.3.5-.5.6l.9-4.9c.1-.2.3-.5.5-.6zm-.1-.6h-.2l-.5.2c-.2.1-.5.4-.5.6l-1 5.1c0 .2 0 .3.1.4l-.2-.1-2.1-1.2-.4-.2-3.2-1.8c-.1-.1-.1-.2-.1-.4l1-5.1c.1-.3.3-.6.5-.6l.5-.2h.2l5.9 3.3zm-1.7 10.1v.4c0 .3-.2.7-.5.9l-6.4 3.7v-.4c0-.3.2-.7.5-.9l6.4-3.7z"/>
        <path class="st222" d="M1386.9 129.2v.4l-6.5 3.7c-.3.2-.5.6-.5.9v.4l-.3.2c-.2.1-.3.1-.4 0-.1-.1-.1-.2-.1-.3v-.8c0-.3.2-.7.5-.9l6.8-3.9c.1-.1.3-.1.3 0 .2 0 .2.1.2.3z"/>
        <path class="st226" d="M1386.8 128.8c-.1 0-.2 0-.4.1l-6.8 3.9c-.3.2-.5.6-.5.9v.8c0 .1 0 .3.1.3l-5.9-3.4c-.1 0-.2-.2-.2-.3v-.8c0-.3.2-.7.5-.9l6.8-3.9c.1-.1.2-.1.3-.1h.1l2.1 1.2.4.2 2.2 1.3.4.2.9.5z"/>
        <path class="st92" d="M1386.7 125.8l-.2 1.1c-.1.5-.3 1-.7 1.4l-.4-.2c.3-.3.5-.7.5-1l.3-1.4.2.1h.3zm-2.6-1.4l-.2 1c-.1.5-.3 1-.7 1.4l-.4-.2c.3-.3.5-.7.5-1l.3-1.4.5.2z"/>
      </g>
      <g id="XMLID_3_">
        <path class="st223" d="M1395.4 130.4v2.6c0 .8-.6 1.8-1.3 2.2l-5.1 3c-.3.2-.6.2-.8.1h-.1s-.1 0-.1-.1c-.2-.2-.2-.6-.1-1 .7-2.4 3.2-5.4 6.2-7.4.3-.2.7-.3.9-.2h.1c.2.2.3.4.3.8zm-.8 3.1v-2.6c0-.3-.2-.4-.4-.2-.2.1-.3.2-.5.3-2.1 1.5-3.9 3.5-4.7 5.2-.1.3-.3.6-.3.9v.1s.1.1.3 0l5.1-3c.3-.1.5-.4.5-.7z"/>
        <path class="st218" d="M1394.2 129.2l.8.4c-.2-.1-.6-.1-.9.2-3 2-5.5 5-6.2 7.4-.1.4-.1.8.1 1l.1.1-.8-.4h-.1s-.1 0-.1-.1c-.2-.2-.2-.6-.1-1 .7-2.4 3.1-5.4 6.2-7.4.5-.4.8-.4 1-.2z"/>
        <path class="st214" d="M1394.6 132.5v1c0 .3-.2.6-.4.7l-5.1 3c-.1.1-.2.1-.3 0v-.1l.3-.9 4.2-2.4c.2-.1.4-.5.4-.7v-2c.2-.1.3-.2.5-.3.2-.1.4 0 .4.2v1.5z"/>
      </g>
      <path class="st214" d="M1375.1 135.6c-.2-.1-.4-.1-.6.1l-.6.3 1.3.8 2.1 1.2.6-.3c.2-.1.4-.1.6-.1l-3.4-2z"/>
      <path class="st92" d="M1378.8 138.1c0 .2 0 .4-.1.6l-1.3-.8.6-.3c.2-.1.4-.1.6-.1.1.1.2.3.2.6zm-1.6-.8s-.2.1-.5-.1c-.2-.1 0-.3 0-.3l6.2-9.5.5.3-6.2 9.6z"/>
      <path class="st92" d="M1385.9 129.8c-.1 0-.3-.1-.5-.2h-.1c-.3-.1-.7-.4-1-.5h-.1c-.3-.2-1-.6-1.4-.8-.4-.2-1.1-.7-1.4-.9h-.1c-.3-.2-.7-.5-1-.7l-.1-.1c-.2-.2-.5-.4-.3-.7.1-.1.2-.1.3-.1.1 0 .3.1.5.2h.1c.3.1.7.4 1 .5h.1c.3.2 1 .6 1.4.8.4.2 1.1.7 1.4.9h.1c.3.2.7.5 1 .7h.1c.3.2.5.4.4.6-.1.2-.3.3-.4.3z"/>
      <g id="XMLID_16_">
        <path class="st228" d="M1376.3 138.5l-.2 1.1-12.6-7.3.6-.4.1-.4z"/>
        <path class="st216" d="M1376.1 139.6l-.1.4-12.8-7.4-.2-.5z"/>
        <path class="st228" d="M1364.2 131.5l-.1.4-.6.4-.2-.1z"/>
      </g>
      <path class="st216" d="M1362.3 132.1c0-.1.3-4.3.7-7.3.5-4 3.3-7.8 5.6-9.4 4.3-2.9 36-19.8 36.2-19.8l1.1-.6c.8-.3 2.4-.9 4.3.2 1.2.7 1.9 2.1 2.2 4l-.8.1c-.2-1.5-.8-2.7-1.8-3.3-1.3-.8-3.3 0-3.5 0-.9.5-33.2 18.2-36.8 20.4-5 3-6.1 16.2-6.1 16.2l-1.1-.5z"/>
      <path class="st215" d="M1363.3 132.2c0-.4.3-4.4.7-7.5.5-4 3.5-7.9 5.8-9.3 3.6-2 36.7-19.8 36.9-19.9.1 0 2.1-1 3.7-.1 1.1.6 1.8 2.5 1.9 4.4l-1 .4c-.1-1.5-.7-3.4-1.5-3.9-1-.6-2.5.1-2.6.1-.6.3-31.7 17.7-35.5 19.2-7.8 3-7.5 15.6-7.5 15.7l-.9.9z"/>
      <path class="st216" d="M1375.7 139.9c0-.1-.2-2 .2-5 .5-4 3-10.1 5.9-11.7 4.6-2.4 36.2-19.8 36.3-19.8l1.1-.6c.8-.3 1.8-1.1 4.9.5 1.3.7 2.9 16.9 3.2 18.8l-.7-.5c-.8-4.7-2.1-16-3.1-17.2-1-1.1-2.6-.2-2.9-.1-.9.5-34.3 17.8-37.9 19.9-5 3-5.9 16.2-5.9 16.2l-1.1-.5z"/>
      <path class="st216" d="M1413.1 108.5c1.6-.9 3.4-1.5 4.8-2.6 1.4-1 3.1-2.1 4.8-2.2.3 0 .5.1.7.3.6-.3.7-.6.7-.6l-14.1-8.1-2.5-.6c-.6.3-34.8 18.8-38.6 21.1 0 0-2.4 1.9-2.9 2.9l14.6 7.1-.1.4c.6-.5 1.4-2 2.2-2.4.7-.3 17.9-8.7 29.9-14.6.1-.3.2-.6.5-.7z"/>
      <path class="st229" d="M1366.6 118.6s8.1 2.6 13.2 6.6c0 0-.5.5-.9 1.2 0 0-5.7-4.2-13.1-6.5 0 0 .3-.8.8-1.3z"/>
      <linearGradient id="SVGID_9_" gradientUnits="userSpaceOnUse" x1="1371.091" y1="119.872" x2="1371.091" y2="139.386">
        <stop offset="0" stop-color="#FFF" stop-opacity="0"/>
        <stop offset="1" stop-opacity=".4"/>
      </linearGradient>
      <path class="st230" d="M1363.3 132.2s.4-10.2 2.5-12.4c0 0 7.9 2.3 13.1 6.5 0 0-3.4 4.6-3.2 13l-12.4-7.1z"/>
      <path class="st215" d="M1376.8 140.5c0 .6-.2-2.6.2-5.7.5-4 2.9-9.8 6.2-11.6 3.7-2 36.9-19.8 37-19.9.1 0 2.1-1 3.7-.1 1.1.6 1.6 2.2 1.8 4.7l-.8.2c-.5-3.1-.8-3.6-1.6-4-1-.6-2.5.2-2.7.3-.6.3-33.4 18-37 19.9-6.1 3.1-6 15.4-6 15.5l-.8.7z"/>
      <path class="st215" d="M1425 107.7h.8l2.2 13.9-.7.5z"/>
    </g>
    <g id="car-blue">
      <path class="st16" d="M1211.8 1514.6l-70.6 40.7 28.4 16.6 71.3-40.9z"/>
      <g class="st14">
        <path class="st231" d="M1196.1 1567.4c0 3.6-2.5 7.9-5.6 9.7-3.1 1.8-5.6.3-5.6-3.2 0-3.6 2.5-7.9 5.6-9.7 3.1-1.9 5.6-.4 5.6 3.2z"/>
        <path class="st231" d="M1186.8 1561.9c1.6-.9 3-1 4-.4l4.1 2.5c-1-.6-2.6-.4-4.2.5-3.1 1.8-5.6 6.1-5.6 9.7 0 1.8.5 2.7 1.5 3.3l-3.7-2.3c-1-.6-1.6-1.8-1.6-3.6-.2-3.6 2.3-7.9 5.5-9.7z"/>
      </g>
      <g class="st14">
        <path class="st231" d="M1238.5 1543c0 3.6-2.5 7.9-5.6 9.7-3.1 1.8-5.6.3-5.6-3.2 0-3.6 2.5-7.9 5.6-9.7 3.1-1.9 5.6-.4 5.6 3.2z"/>
        <path class="st11" d="M1232.9 1549.5c1.6-.9 2.8-3.1 2.8-4.9 0-1.8-1.3-2.5-2.9-1.6-1.6.9-2.8 3.1-2.8 4.9.1 1.7 1.4 2.5 2.9 1.6z"/>
        <path class="st231" d="M1229.2 1537.5c1.6-.9 3-1 4-.4l4.1 2.5c-1-.6-2.6-.4-4.2.5-3.1 1.8-5.6 6.1-5.6 9.7 0 1.8.5 2.7 1.5 3.3l-3.7-2.3c-1-.6-1.6-1.8-1.6-3.6-.1-3.6 2.4-7.9 5.5-9.7z"/>
      </g>
      <path class="st20" d="M1155.8 1556.5v2l23.4 14v-2c0-2.4-.3-4.1 1.8-5.6l9.5-7.8c2.1-1.5 5.4-4.9 6.4-7.6l1.4-3.8c1-2.7 2.6-5.8 4.7-7.1l22.3-12.8c2.1-1.2 4.2-.6 4.8 1.4l.5 1.7s1.7 2.5 4.7 2l7.6-2.8-22.6-13.1c-.7-.4-1.5-.4-2.5 0l-2.1.9-8.5-4.9c-.9-.5-2.3-.5-3.6.2l-22.2 12.8c-2.1 1.2-4.6 4.4-5.5 7l-1.4 3.9c-1 2.7-3.4 6.1-5.5 7.6l-9.5 7c-2 1.4-3.7 4.6-3.7 7z"/>
      <path class="st21" d="M1191.6 1555.6c2.1-1.5 4.5-4.9 5.5-7.6l1.4-3.8c1-2.7 3.4-5.8 5.5-7.1l22.3-12.8c2.1-1.2 4.2-.6 4.8 1.4l.6 2c.6 2 2.7 2.9 4.8 2l3.9-1.7c2.1-.9 3.8.4 3.8 2.8v2.9c-.1 0-.2.1-.3.1l-1.3.7c-.8.5-1.5 1.7-1.5 2.6v1.5c0 .8.5 1.2 1.2 1l-3.7 2.1c0-4.1-3-5.8-6.6-3.7-3.6 2.1-6.5 7.1-6.6 11.3l-28.2 16.3c0-4.1-3-5.8-6.6-3.7-3.6 2.1-6.5 7.1-6.5 11.3l-4.2 2.4c.7-.6 1.2-1.6 1.2-2.4v-1.5c0-1-.7-1.3-1.5-.9l-1.1.6v-2.1c0-2.4 1.7-5.6 3.7-7.1l9.4-6.6z"/>
      <path class="st10" d="M1199.8 1544l-2.5 8.3c-.1.2 0 .4.1.5.1.1.2.1.3.1.1 0 .2 0 .2-.1l15.4-8.9c.1-.1.2-.2.2-.4v-9.5c0-.1-.1-.3-.2-.4-.1-.1-.3-.1-.4 0l-9 5.2c-1.5.9-3.4 3.3-4.1 5.2zm16-11.8v9.5c0 .2.1.3.2.4h.4l8.1-4.7c.1-.1.2-.2.2-.4v-9.5c0-.2-.1-.3-.2-.4-.1-.1-.3-.1-.4 0l-8.1 4.7c-.1.1-.2.2-.2.4zm9.5-5.5v9.5c0 .1.1.3.2.4.1 0 .1.1.2.1s.1 0 .2-.1l4.3-2.5c.2-.1.2-.3.2-.5l-1.5-6.1c-.3-1-1.1-1.6-2.1-1.6-.4 0-.9.1-1.3.3-.2.2-.2.4-.2.5zm-52.8 13.8c0 .1.1.2.2.3l18.9 11c.1 0 .1.1.2.1s.2-.1.3-.2c1.3-1.6 2.5-3.5 3-5 .2-.8.4-1.5.7-2.1l.7-1.9c.1-.3.2-.6.4-.9.1-.2 0-.4-.2-.6l-19-11.1c-.1-.1-.2-.1-.3 0-.1 0-.2.1-.3.2-.1.3-.3.6-.4.9l-1.4 3.8c-.5 1.5-1.6 3.4-2.8 5v.5z"/>
      <path class="st232" d="M1213 1543.6v-9.5l-9 5.2c-1.4.8-3.2 3.1-3.9 4.9l-2.5 8.3 15.4-8.9zm3.3-1.9l8.1-4.7v-9.5l-8.1 4.7v9.5zm9.4-5.5l4.3-2.5-1.5-6.1c-.3-1.1-1.6-1.6-2.8-1v9.6z"/>
      <path class="st233" d="M1221 1542.6l2-1.1c.3-.2.6-.7.6-1.1 0-.4-.3-.6-.6-.4l-2 1.2c-.3.2-.6.7-.6 1.1-.1.4.2.5.6.3zm-12.8 7.4l2-1.2c.3-.2.6-.7.6-1.1 0-.4-.3-.5-.6-.4l-2 1.2c-.3.2-.6.7-.6 1.1-.1.5.2.6.6.4z"/>
      <path class="st232" d="M1172.9 1540.4c1.2-1.6 2.3-3.5 2.9-5.1l1.4-3.9c.1-.3.2-.6.4-.9l19 11.1c-.2.3-.3.7-.4 1l-.7 1.8c-.3.6-.6 1.3-.8 2.1-.6 1.6-1.7 3.4-3 4.9l-18.8-11z"/>
      <path class="st233" d="M1172.5 1566c0-.6.4-.9 1-.6l2.9 1.7c.5.3.9 1 .9 1.6 0 .6-.4.8-1 .5l-2.9-1.6c-.4-.3-.9-1-.9-1.6zm-16.1-9.4c0-.6.4-.8 1-.5l2.9 1.7c.5.3 1 1 1 1.6 0 .6-.4.8-1 .5l-2.9-1.7c-.6-.3-1-1-1-1.6z"/>
      <path class="st11" d="M1190.5 1573.9c1.6-.9 2.8-3.1 2.8-4.9 0-1.8-1.3-2.5-2.8-1.6-1.6.9-2.8 3.1-2.8 4.9-.1 1.7 1.2 2.5 2.8 1.6z"/>
      <path class="st14 st234" d="M1242.5 1534.6c-.8.5-1.5 1.7-1.5 2.6v1.5c0 .8.5 1.2 1.2 1 .1 0 .2-.1.4-.2l1.3-.7c.8-.5 1.5-1.7 1.5-2.6v-1.5c0-.9-.5-1.3-1.2-1-.1 0-.2.1-.3.1l-1.4.8zm-64 36.8c-.8.5-1.5 1.6-1.5 2.6v1.5c0 1 .7 1.3 1.5.9l1.3-.7c.1-.1.2-.2.4-.3.7-.6 1.2-1.5 1.2-2.4v-1.5c0-1-.7-1.3-1.5-.9l-1.1.6-.3.2z"/>
      <path class="st234" d="M1154.5 1560.9v1.5c0 .5.2.8.4 1 7.5 4.4 15 8.7 22.6 13.1-.3-.2-.5-.5-.5-1v-1.5c0-1 .7-2.1 1.5-2.6l-22.6-13.1c-.8.5-1.4 1.7-1.4 2.6z"/>
      <path class="st11" d="M1163.2 1567.8v-2.3l5.1 2.9v2.4z"/>
    </g>
    <g id="coffee-house">
      <path class="st16" d="M703.7 1983.9c0-21.1-28.8-38.2-64.4-38.2-35.6 0-64.4 17.1-64.4 38.2 0 14.4 13.4 26.9 33.2 33.4l51.5 29.9v-27.1c25.7-5 44.1-19.3 44.1-36.2z"/>
      <path class="st11" d="M727.1 1965.8l-52.3 29.4v60.8l52.4-30.3z"/>
      <path class="st20" d="M702.3 2030.6l19.7-11.3-.1-22.6-19.6 11.3z"/>
      <path class="st29" d="M679.8 2052.9l16.5-9.5-.1-36.3-16.5 9.5z"/>
      <path class="st11" d="M697 2043.1l-.1-37.2-17.8 10.3.1 37.2 17.8-10.3zm-1.4-.1l-15.1 8.7-.1-34.7 15.1-8.7.1 34.7z"/>
      <path class="st235" d="M674.8 1981.8v74.2l-52.1-30.3V1961z"/>
      <path class="st29" d="M739.5 1972.2c0 21.1-28.8 38.2-64.4 38.2-35.6 0-64.4-17.1-64.4-38.2s28.8-38.2 64.4-38.2c35.5 0 64.4 17.1 64.4 38.2z"/>
      <ellipse class="st236" cx="675.1" cy="1972.2" rx="55.7" ry="33"/>
      <path class="st29" d="M705.6 1972.2c0 10-13.6 18.1-30.5 18.1-16.8 0-30.5-8.1-30.5-18.1 0-10 13.6-18.1 30.5-18.1 16.8 0 30.5 8.1 30.5 18.1z"/>
      <path class="st237" d="M702.7 1970.4c0 9-12.4 16.4-27.6 16.4-15.2 0-27.6-7.3-27.6-16.4 0-9 12.4-16.4 27.6-16.4 15.2.1 27.6 7.4 27.6 16.4z"/>
      <path class="st29" d="M702.7 1900c-16.7-9.9-45.1-10.1-59.6 3.2-1.2 0-4.7 5-4.9 6.2-.6 1.2-1.3 2.9-1.3 4.2 0 12.7 2 25.8 2.5 38.6-.5-15.8 22.5-20.8 34.3-21 12.1-.2 37.6 4.5 36.8 21.2.4-9.9 1.4-19.7 2.3-29.5.2-2.5.7-5.1.6-7.6 0-6.8-5.2-12-10.7-15.3-.4-.3 7.6 4.5 0 0z"/>
      <path class="st21" d="M713.6 1922.8c0 12.6-17.2 22.8-38.4 22.8s-38.3-10.2-38.3-22.8c0-12.6 17.2-22.8 38.3-22.8 21.2.1 38.4 10.3 38.4 22.8z"/>
      <ellipse class="st238" cx="664.8" cy="1911.5" rx="13.3" ry="8"/>
      <path class="st238" d="M698.9 1929.5c0 2.5-3.2 4.5-7.3 4.5-4 0-7.2-2-7.2-4.5s3.2-4.5 7.2-4.5 7.3 2 7.3 4.5z"/>
      <path class="st239" d="M718.1 1917.2c-1.1 10.4-20.4 20.2-41.3 20.5-21.3.4-43.4-9.5-44.5-20.8.5 4.9.8 9.8 1.2 14.7.3 3.9.6 7.7.9 11.6.1 1.8.2 3.5.3 5.3.1.8.1 1.6.1 2.3 0 .3.1 3 .1 1.5 2.5 38.8 68.4 42.6 79.1 7 .7-2.3 1.1-4.5 1.2-6.8 1-10.2 1.7-23.7 2.9-35.3 0 .4 0 .3 0 0z"/>
      <path class="st29" d="M667.8 1983.4v-46c-18.1-2-34.5-10.7-35.4-20.3.5 4.9.8 9.8 1.2 14.7.3 3.9.6 7.7.9 11.6.1 1.8.2 3.5.3 5.3.1.8.1 1.6.1 2.3 0 .1.1 1.1.1 1.6 1.2 17.9 16.1 28.3 32.8 30.8z"/>
      <path class="st29" d="M646.4 1974.4l-.7-43.3c-7.6-3.8-12.9-8.8-13.4-14.1.5 4.9.8 9.8 1.2 14.7.3 3.9.6 7.7.9 11.6.1 1.8.2 3.5.3 5.3.1.8.1 1.6.1 2.3 0 .1.1 1.1.1 1.6.7 9.4 5.1 16.7 11.5 21.9z"/>
      <path class="st29" d="M675.3 1890.8c-23.7 0-42.9 11.1-42.9 24.9 0 13.7 19.2 24.9 42.9 24.9s42.9-11.1 42.9-24.9c0-13.7-19.3-24.9-42.9-24.9zm0 46.9c-21.2 0-38.3-9.9-38.3-22.2 0-12.3 17.2-22.2 38.3-22.2 21.2 0 38.3 9.9 38.3 22.2 0 12.2-17.2 22.2-38.3 22.2z"/>
      <path class="st29" d="M712.8 1925.8l-.7 38.8c1.9-3.6 3.1-7.6 3.4-12.1 0-.5.1-1.5.1-1.6 0-.8.1-1.5.1-2.3.1-1.8.2-3.5.3-5.3.3-3.9.6-7.7.9-11.6.4-4.9.7-9.8 1.2-14.7-.3 3.1-2.2 6.1-5.3 8.8zm-77.8 26.7c0-.1-.1-.1 0 0 0 .5 0 .3 0 0z"/>
      <path class="st29" d="M635 1952.5c0-.1-.1-.1 0 0 0 .5 0 .3 0 0z"/>
      <path class="st240" d="M661.8 1939l.4-.2s-.1 0-.1.1c-.2 0-.2.1-.3.1z"/>
      <path class="st29" d="M706.1 1976c-2.7 0-5.7-.7-9-2.2-1.4-.6-2.1-2.2-1.5-3.7.6-1.4 2.2-2.1 3.7-1.5 4 1.7 7.3 2.1 9.6 1.2 1.8-.8 2.7-2.4 3.1-3.5 1.5-4 .5-10.2-2.2-14.1-.8-1.2-1.8-2.1-2.8-2.7-1.6-.9-3.5-1.1-5.5-.6-1.5.4-3-.5-3.4-2-.4-1.5.5-3 2-3.4 3.5-.9 6.8-.4 9.7 1.2 1.8 1 3.3 2.5 4.6 4.3 3.8 5.4 5 13.5 2.9 19.2-1.1 3.1-3.3 5.5-6.1 6.8-1.7.7-3.3 1-5.1 1z"/>
      <path class="st237" d="M714.3 1949.1c-1.3-1.9-2.8-3.3-4.6-4.3-2.9-1.6-6.2-2.1-9.7-1.2-.8.2-1.4.7-1.8 1.4 3.4-.8 6.8-.4 9.6 1.2 1.8 1 3.3 2.5 4.6 4.3 3.8 5.4 5 13.5 2.9 19.2-.7 1.8-1.7 3.4-3 4.6 2.2-1.3 3.9-3.4 4.8-6 2.2-5.8.9-13.9-2.8-19.2zm-16.9 21c4 1.7 7.3 2.2 9.5 1.2.8-.3 1.4-.9 1.9-1.4h-.1c-2.2 1-5.5.5-9.6-1.2-1.4-.6-2.9 0-3.5 1.3.7-.1 1.3-.1 1.8.1z"/>
    </g>
    <g id="golf-kart-2">
      <path class="st211" d="M-90.7 1725.3l16.8-10.2 6.6 4-2 1.2-16.8 10.2-4.6-2.8-2-1.2z"/>
      <g id="XMLID_32_">
        <path class="st212" d="M-83.1 1724.1c-.1.1-.1.1-.1.2.2 0 .5.1.8.3l7.6 4.6 11.7 7.1c1.1.7 2 2.3 2 3.6v4.5l1-.6v-4.5c0-1.3-.9-2.9-2-3.6l-19.4-11.7c-.3-.2-.6-.3-.8-.3-.3 0-.5.2-.8.4z"/>
        <path class="st159" d="M-82.3 1723.7c.2 0 .5.1.8.3l19.4 11.7c1.1.7 2 2.3 2 3.6v4.5l14.8-9v-4.5c0-1.3-.9-2.9-2-3.6l-11.7-7.1-7.6-4.6c-.3-.2-.5-.3-.8-.3l-14.9 9z"/>
        <path class="st212" d="M-67.3 1714.6c-.1.1-.1.1-.1.2.2 0 .5.1.8.3l7.6 4.6 11.7 7.1c1.1.7 2 2.3 2 3.6v4.5l1-.6v-4.5c0-1.3-.9-2.9-2-3.6l-19.4-11.7c-.7-.5-1.2-.3-1.6.1z"/>
      </g>
      <g id="XMLID_31_">
        <path class="st159" d="M-57 1701.4v19.5l1.1.7V1702z"/>
        <path class="st213" d="M-57 1701.4l1.1.6 1-.6-1.1-.6z"/>
        <path class="st213" d="M-55.9 1702v19.6l1-.6v-19.6z"/>
      </g>
      <g id="XMLID_30_">
        <path class="st159" d="M-16.8 1754.6c0 2.6 1.8 5.8 3.9 7.1 1.1.7 2.1.7 2.8.3.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3-.7.3-1.1 1.2-1.1 2.6zm3.9 5.3c-1.4-.8-2.5-2.8-2.5-4.5 0-1.1.5-1.8 1.3-1.8.4 0 .8.1 1.2.4 1.4.8 2.5 2.8 2.5 4.5 0 .5-.1.9-.3 1.2-.4.6-1.3.8-2.2.2z"/>
        <path class="st214" d="M-12.7 1750.1l-3 1.8c.7-.4 1.7-.3 2.8.3 2.2 1.3 3.9 4.5 3.9 7.1 0 1.3-.4 2.2-1.1 2.6l3-1.8c.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2.1-.7-2.8-.3z"/>
        <path class="st214" d="M-15.4 1755.5c0 1.6 1.1 3.6 2.5 4.5.9.6 1.8.4 2.2-.2-.4 0-.8-.1-1.2-.3-1.4-.8-2.5-2.8-2.5-4.5 0-.5.1-.9.3-1.2-.8-.1-1.3.5-1.3 1.7z"/>
        <path class="st92" d="M-14.1 1753.6c-.2.3-.3.7-.3 1.2 0 1.6 1.1 3.6 2.5 4.5.4.3.8.4 1.2.3.2-.3.3-.7.3-1.2 0-1.6-1.1-3.6-2.5-4.5-.4-.2-.8-.3-1.2-.3z"/>
      </g>
      <g id="XMLID_29_">
        <path class="st215" d="M-74.3 1711.1l-.9 6 .8.6.9-6c.2-1.3.9-2.2 1.8-2.4.5-.1 1.1 0 1.7.3l3 1.9v1.9c0 .8.5 1.7 1.1 2.1l4.5 2.8c.3.2.6.2.8.1 0 0 .1 0 .1-.1.2-.2.2-.5.1-.9-.6-2.3-2.8-5.1-5.5-6.9-.3-.2-.6-.3-.8-.1h-.1c-.1.1-.2.2-.2.3l-3-1.9c-.8-.5-1.6-.6-2.2-.4-.2 0-.3.1-.4.2l-.1.1c-.9.4-1.4 1.2-1.6 2.4zm8 2.8v-2.4c0-.2.1-.3.3-.2.2.1.4.3.6.5 1.6 1.2 3 2.8 3.7 4.3.2.4.4.8.5 1.2v.1s-.1.1-.3 0l-4.5-2.8c-.1-.2-.3-.5-.3-.7z"/>
        <path class="st216" d="M-73.6 1711.7l-.9 6 1-.6.9-6c.1-.8.4-1.4.8-1.8-.8.2-1.5 1.1-1.8 2.4z"/>
        <path class="st217" d="M-72 1708l-.8.5c.1-.1.3-.1.4-.2.7-.2 1.5-.1 2.2.4l3 1.9c.1-.1.1-.2.2-.3h.1l.6-.3-2.9-1.8c-1-.6-1.9-.6-2.7-.2h-.1z"/>
        <path class="st218" d="M-65.8 1709.7l-.3.2-.6.3c.2-.1.5-.1.8.1 2.7 1.9 4.9 4.7 5.5 6.9.1.4.1.7-.1.9 0 0 0 .1-.1.1l.9-.6.1-.1c.2-.2.2-.5.1-.9-.6-2.3-2.8-5.1-5.5-6.9-.3-.1-.6-.2-.8 0z"/>
        <path class="st214" d="M-66.3 1711.5v2.4c0 .3.2.6.4.7l4.5 2.8c.1.1.2.1.3 0v-.1c-.1-.4-.3-.8-.5-1.2l-3.3-2c-.2-.1-.4-.4-.4-.7v-1.6c-.2-.2-.4-.3-.6-.5-.3-.2-.4 0-.4.2z"/>
      </g>
      <g id="XMLID_28_">
        <path class="st219" d="M-82.6 1721.6v.9c0 .4.3.9.6 1.1l7.9 4.8c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.2-.2.3-.2.5z"/>
        <path class="st220" d="M-82.4 1721.2c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l2.6-1.6-.2-.3c-.1.1-.2.1-.3.1v-.6c.1 0 .2-.1.2-.3l.6-2.7-2.8 1.7-.1.1c-.1 0-.3 0-.4-.2l-.6-.6c-.3-.2-.4-.7-.4-.9l1.1-4.3h-.1c-.3-.2-.6-.7-.6-1.1v-.5l-.4-.2c-.2-.1-.3-.1-.4 0l-7 4.1z"/>
        <path class="st219" d="M-75.1 1723.2c-.1.3.1.7.4.9l.6.6c.1.1.3.2.4.2l.1-.1.1-.1 1.2-4.7-1.7-1-1.1 4.2z"/>
        <path class="st220" d="M-74.7 1717.3v.5c0 .4.3.9.6 1.1h.1l.3-1-1-.6z"/>
        <path class="st221" d="M-74.7 1716.9v.5l.9.6.3-1-.6-.3c-.2-.1-.3-.1-.4-.1-.1-.1-.2 0-.2.3z"/>
        <path class="st220" d="M-74.5 1716.4c.1 0 .3 0 .4.1l.6.3.1-.2c0-.1 0-.1.1-.2l.1-.1 6.4-3.9-.3-.2c-.2-.1-.3-.1-.4 0l-7 4.2z"/>
        <path class="st219" d="M-73.8 1717.9l-.3 1 1.7 1 .3-1zm.2-1.1l-.3 1 1.7 1 .2-.9v-.2l-1.6-.9z"/>
        <path class="st222" d="M-73.6 1724.8l2.8-1.7.1-.5c.1-.3 0-.9-.2-1.3l-.1-.1.1-.4-1.5-.9-1.2 4.7c.1.1 0 .2 0 .2z"/>
        <path class="st219" d="M-73.5 1716.6l-.1.2 1.7 1c0-.3-.2-.5-.4-.7l-.6-.6c-.1-.1-.3-.2-.4-.2l-.1.1c0 .1-.1.1-.1.2z"/>
        <path class="st222" d="M-66.9 1712.5l-6.4 3.9c.1 0 .3 0 .4.2l.6.6c.2.2.3.5.4.7l4.2 2.5c0-.3-.1-.6-.3-.8l-.1-.1.1-.5.2.5c.2.4.3.8.4 1.2l.3.2.3-.2.1-.1.2-.7-.4-.4c-.3-.2-.4-.7-.4-.9l1.3-5.3-.9-.8zm-5.2 6.4l-.3 1 1.5.9v-.1l.1.2 1.8 1.1 1-.6z"/>
        <path class="st222" d="M-72.1 1718.9l4.1 2.5.2-.1.1-.5v-.4l-4.2-2.5v.2l-.2.8z"/>
        <path class="st92" d="M-71.6 1726.1v.6c.1 0 .2 0 .3-.1.1-.1.2-.2.3-.4l.7-3.2v-.2l-.5.3-.6 2.7c0 .1-.1.2-.2.3z"/>
        <path class="st220" d="M-71.3 1726.6l.2.3 4.2-2.6c.1-.1.2-.2.2-.4v-.5l-1-.6-.3 1.6c-.1.3-.3.5-.6.5v-.6c.1 0 .2-.1.2-.3l.3-1.5-.9-.5-1.3.8v.2l-.7 3.2c0 .1-.1.3-.3.4z"/>
        <path class="st92" d="M-70.9 1720.8l-.1.4.1.1c.2.4.3 1 .2 1.3l-.1.5.5-.3c0-.5-.1-1.1-.4-1.6l-.1-.3-.1-.1zm0-.1v.1l.1.1z"/>
        <path class="st222" d="M-70.8 1720.9l.1.3c.3.5.4 1.1.4 1.6l1.3-.8-1.8-1.1z"/>
        <path class="st220" d="M-69 1722l.9.5.2-1-.1-.1z"/>
        <path class="st92" d="M-68.6 1724.3v.6c.3 0 .5-.2.6-.5l.3-1.6-.4-.2-.3 1.5-.2.2zm.7-2.8l-.2 1 .4.3.2-1.1zm0-2.6l-.1.5.1.1c.1.2.2.6.3.8l.4.2c0-.4-.2-.9-.4-1.2l-.3-.4z"/>
        <path class="st222" d="M-68 1721.4l.1.1.1-.2z"/>
        <path class="st92" d="M-67.8 1721.3v.2l.4.2.1-.6v-.2l-.5.4z"/>
        <path class="st92" d="M-67.7 1720.8l-.1.5.5-.3v-.4l-.4-.2v.4z"/>
        <path class="st220" d="M-67.5 1721.7l-.2 1 1 .6v-.5c0-.4-.3-.9-.6-1.1h-.2z"/>
        <path class="st221" d="M-67.3 1721.2l-.1.6.2.1c.3.2.6.7.6 1.1v.5l.4.2c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-.7-.4-.3.2c-.1-.1-.1 0-.1.1z"/>
        <path class="st222" d="M-67 1720.8l-.3-.2v.4l.3-.2zm-.2-2.4c-.1.3.1.7.4.9l.4.4 1.4-5.9v-.2l-.9-.6-1.3 5.4z"/>
        <path class="st220" d="M-67 1720.8l.7.4c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l2.6-1.6-.2-.3c-.1.1-.2.1-.3.1v-.6c.1 0 .2-.1.2-.3l.6-2.7-2.8 1.7-.1.1c-.1 0-.3 0-.4-.2l-.2-.2-.2.7c0 .1 0 .1-.1.1l-.3.4z"/>
        <path class="st222" d="M-66.5 1712.3l-.4.2 1 .6.1-.6-.2-.2c-.2-.1-.3-.2-.4-.2l-.1.2z"/>
        <path class="st219" d="M-65 1713.9l-1.4 5.9.2.2c.1.1.3.2.4.2l.1-.1.1-.1 1.4-5.7-.8-.5v.1z"/>
        <path class="st222" d="M-65.8 1712.6l-.1.6.9.6c0-.3-.2-.5-.4-.7l-.4-.5z"/>
        <path class="st219" d="M-65.6 1711.8l-.2.7.4.4c.2.2.3.5.4.7l.8.5.2-.9c.1-.3-.1-.7-.4-.9l-.6-.6c-.1-.1-.3-.2-.4-.2l-.1.1c-.1.1-.1.2-.1.2z"/>
        <path class="st222" d="M-65.7 1720l2.8-1.7.1-.5c.1-.3 0-.9-.2-1.3l-.1-.1.1-.5.2.5c.3.5.4 1.1.4 1.6l2.3-1.4-4.1-2.5-1.4 5.7c-.1.1-.1.2-.1.2z"/>
        <path class="st222" d="M-58.6 1707.5l-6.8 4.1c.1 0 .3 0 .4.2l.6.6c.3.2.4.7.4.9l-.2.9 4.1 2.5.2-.1.1-.5c.1-.3 0-.9-.2-1.3l-.1-.1.1-.5.2.5c.3.5.4 1.1.4 1.6l.6-.4.1-.1 1.6-6.6c.1-.3-.1-.7-.4-.9l-.6-.6c-.2-.1-.3-.2-.4-.2h-.1z"/>
        <path class="st92" d="M-63.7 1721.3v.6c.1 0 .2 0 .3-.1.1-.1.2-.2.3-.4l.7-3.2v-.2l-.5.3-.6 2.7c0 .2-.1.3-.2.3z"/>
        <path class="st220" d="M-63.4 1721.8l.2.3 4.2-2.6c.1-.1.2-.2.2-.4v-1c0-.4-.3-.9-.6-1.1l-.2-.1-.6 2.6c-.1.3-.3.5-.6.5v-.6c.1 0 .2-.1.2-.3l.5-2.5-.1-.1-2.3 1.4v.2l-.7 3.2c.1.3 0 .4-.2.5z"/>
        <path class="st92" d="M-63 1715.9l-.1.5.1.1c.2.4.3 1 .2 1.3l-.1.5.5-.3c0-.5-.1-1.1-.4-1.6l-.2-.5zm2.3 3.6v.6c.3 0 .5-.2.6-.5l.6-2.6-.4-.2-.5 2.5c-.1.1-.2.2-.3.2zm.7-5.4l-.1.5.1.1c.2.4.3 1 .2 1.3l-.1.5.5-.3c0-.5-.1-1.1-.4-1.6l-.2-.5z"/>
        <path class="st92" d="M-59.9 1716.5v.2l.4.2.1-.6v-.2l-.5.4z"/>
      </g>
      <path class="st217" d="M-83.4 1724.3c-.2 0-.5.2-.6.4l7.3 4.4c3.1 1.8 5.6 5.8 6.5 9.7l9.1 5.5v-4.5c0-1.3-.9-2.9-2-3.6l-11.7-7.1-7.6-4.6c-.3-.2-.5-.3-.8-.3-.1.1-.1.1-.2.1z"/>
      <path class="st212" d="M-85 1725.3l7.3 4.4c3.1 1.8 5.6 5.8 6.5 9.7l1-.6c-.9-3.9-3.4-7.8-6.5-9.7l-7.3-4.4-1 .6z"/>
      <path class="st214" d="M-82.6 1732.6c-.2.6-.4 1.3-.4 2.2l2-1.2c0-1.2.3-2.1.7-2.7-1.1 0-1.9.6-2.3 1.7z"/>
      <path class="st214" d="M-83 1734.7c0-.8.1-1.6.4-2.2l-1.5-.9-2-1.2-4.6-2.8-2-1.2v2.4l6.6 4 3.1 1.9z"/>
      <path class="st92" d="M-81 1733.5l8.3 5c-.8-2.8-2.7-5.7-4.9-7-1-.6-1.9-.8-2.7-.8-.5.7-.7 1.7-.7 2.8zm56 26.5c0 .3-.1.5-.2.6h-.1l-1.9 1.1h-.1c-.2.1-.4.1-.7-.1l-1.7-1.1c-1-.6-1.9-.8-2.7-.8-.4.7-.7 1.6-.7 2.7l8.9 3.1c1.1.4 1.6-.5 1.1-2l-.7-2.5c-.1-.4-.5-.9-.7-1.1-.3.2-.5.1-.5.1z"/>
      <path class="st212" d="M-71.2 1739.5l24.8 15.1 6.2 3.7c1.1.7 2.4.6 3-.2l.5-.6c-.5 0-1-.2-1.5-.5l-21.8-13.3-1 .6-9.1-5.5-1.1.7z"/>
      <path class="st214" d="M-32.3 1759.9c-1.6.1-2.7 1.6-2.7 3.9l2-1.2c0-1.1.2-2 .7-2.7z"/>
      <g id="XMLID_27_">
        <path class="st159" d="M-82.6 1736.2c0 2.6 1.8 5.8 3.9 7.1 1.1.7 2.1.7 2.8.3.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3-.6.3-1.1 1.2-1.1 2.6zm3.9 5.3c-1.4-.8-2.5-2.8-2.5-4.5 0-1.1.5-1.8 1.3-1.8.4 0 .8.1 1.2.4 1.4.8 2.5 2.8 2.5 4.5 0 .5-.1.9-.3 1.2-.4.6-1.2.8-2.2.2z"/>
        <path class="st214" d="M-72.9 1741.8c.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3l-3 1.8c.7-.4 1.7-.3 2.8.3 2.2 1.3 3.9 4.5 3.9 7.1 0 1.3-.4 2.2-1.1 2.6l3-1.8z"/>
        <path class="st218" d="M-81.1 1737c0 1.6 1.1 3.6 2.5 4.5.9.6 1.8.4 2.2-.2-.4 0-.8-.1-1.2-.3-1.4-.8-2.5-2.8-2.5-4.5 0-.5.1-.9.3-1.2-.8 0-1.3.6-1.3 1.7z"/>
        <path class="st223" d="M-79.8 1735.2c-.2.3-.3.7-.3 1.2 0 1.6 1.1 3.6 2.5 4.5.4.3.8.4 1.2.3.2-.3.3-.7.3-1.2 0-1.6-1.1-3.6-2.5-4.5-.5-.2-.9-.3-1.2-.3z"/>
      </g>
      <g id="XMLID_26_">
        <path class="st159" d="M-34.6 1765.3c0 2.6 1.8 5.8 3.9 7.1 1.1.7 2.1.7 2.8.3.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3-.6.3-1.1 1.3-1.1 2.6zm4 5.4c-1.4-.8-2.5-2.8-2.5-4.5 0-1.1.5-1.8 1.3-1.8.4 0 .8.1 1.2.4 1.4.8 2.5 2.8 2.5 4.5 0 .5-.1.9-.3 1.2-.5.6-1.3.7-2.2.2z"/>
        <path class="st214" d="M-24.8 1770.9c.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3l-3 1.8c.7-.4 1.7-.3 2.8.3 2.2 1.3 3.9 4.5 3.9 7.1 0 1.3-.4 2.2-1.1 2.6l3-1.8z"/>
        <path class="st218" d="M-33.1 1766.2c0 1.6 1.1 3.6 2.5 4.5.9.6 1.8.4 2.2-.2-.4 0-.8-.1-1.2-.3-1.4-.8-2.5-2.8-2.5-4.5 0-.5.1-.9.3-1.2-.8-.1-1.3.6-1.3 1.7z"/>
        <path class="st223" d="M-31.8 1764.4c-.2.3-.3.7-.3 1.2 0 1.6 1.1 3.6 2.5 4.5.4.3.8.4 1.2.3.2-.3.3-.7.3-1.2 0-1.6-1.1-3.6-2.5-4.5-.5-.2-.9-.4-1.2-.3z"/>
      </g>
      <path class="st224" d="M-85 1725.3c-.5.6-.8 1.8-.9 2.8-.2 1.2-.1 2.3-.1 2.3l2 1.2 1.5.9c.4-1.1 1.3-1.7 2.3-1.8.8-.1 1.7.2 2.7.8 2.2 1.4 4.2 4.2 4.9 7 .2.9.4 1.8.4 2.6l37.4 22.7c0-2.4 1.1-3.8 2.7-3.9.8-.1 1.7.2 2.7.8l1.7 1.1c.3.2.5.2.7.1h.1c.2-.1.2-.3.2-.6v-1.7s-1.7-1-3.8-2.3c-2.1-1.3-3.8-2.3-3.8-2.3l-2.1 2.7-.5.6c-.6.7-2 .8-3 .2l-6.2-3.7-24.8-15.1c-.9-3.9-3.4-7.8-6.5-9.7l-7.6-4.7z"/>
      <g id="XMLID_25_">
        <path class="st223" d="M-82.8 1721v1.9c0 .8.5 1.7 1.1 2.1l4.5 2.8c.3.2.6.2.8.1 0 0 .1 0 .1-.1.2-.2.2-.5.1-.9-.6-2.3-2.8-5.1-5.5-6.9-.3-.2-.6-.3-.8-.1h-.1c-.1.1-.2.2-.2.3m.7 3.2v-2.4c0-.2.1-.3.3-.2.2.1.4.3.6.5 1.6 1.2 3 2.8 3.7 4.3.2.4.4.8.5 1.2v.1s-.1.1-.3 0l-4.5-2.8c-.1-.1-.3-.4-.3-.7z"/>
        <path class="st218" d="M-81.6 1719.3l-.3.2-.6.3c.2-.1.5-.1.8.1 2.7 1.9 4.9 4.7 5.5 6.9.1.4.1.7-.1.9l-.1.1.9-.6.1-.1c.2-.2.2-.5.1-.9-.6-2.3-2.8-5.1-5.5-6.9-.2-.2-.6-.2-.8 0z"/>
        <path class="st214" d="M-82.1 1721v2.4c0 .3.2.6.4.7l4.5 2.8c.1.1.2.1.3 0v-.1c-.1-.4-.3-.8-.5-1.2l-3.3-2c-.2-.1-.4-.4-.4-.7v-1.6c-.2-.2-.4-.3-.6-.5-.2-.1-.4 0-.4.2z"/>
      </g>
      <path class="st212" d="M-29.3 1744.7l2-1.3-17-9.2-1 .6 16.8 9.4-1.2.2z"/>
      <path class="st223" d="M-33.8 1747.4s.1-.1.2-.1l5.2-3.2-16.9-9.4-14.8 8.9 21.8 13.3c.5.3 1 .4 1.5.5l1.7-2.2 1-7.4c.1-.1.1-.3.3-.4z"/>
      <path class="st214" d="M-34.1 1747.9l-1 7.4.4-.5.9-5.5 2-1.2-1.2-.7c-.3-.2-.5-.2-.7-.1l-.2.1c-.1.1-.1.3-.2.5z"/>
      <path class="st159" d="M-19 1738.5l-14.6 8.8c.2-.1.5 0 .7.1l1.2.7 12.3-7.4 2.5-1.5-1.2-.7c-.3-.2-.5-.2-.7-.1l-.2.1z"/>
      <g id="XMLID_24_">
        <path class="st217" d="M-72.7 1710.9v19.6l1 .6v-19.5z"/>
        <path class="st213" d="M-72.7 1710.9l1 .7 1-.6-1.1-.7z"/>
        <path class="st213" d="M-71.7 1711.6v19.5l1-.6V1711z"/>
      </g>
      <path class="st224" d="M-33.7 1749.3l-.9 5.5s1.7 1 3.8 2.3c2.1 1.3 3.8 2.3 3.8 2.3s-.5-3.2-1.8-5c-1.9-2.9-4.9-5.1-4.9-5.1z"/>
      <path class="st225" d="M-16 1754.5l4.8-2.9 1-.6.4.2h.1c.3.2.6.6.7 1.1l.7 2.5c.3 1 .2 1.7-.3 2l-14.6 8.9c.3-.3.4-1 .2-1.9l-.7-2.5c-.1-.4-.5-.9-.7-1.1-.3-.2-.5-.3-.5-.3l8.9-5.4z"/>
      <path class="st159" d="M-10.2 1749.3v1.7l.4.2 1.2-.7c.2-.1.3-.3.3-.7v-1.7s-.5-3.2-1.8-5c-2-3-5-5.1-5-5.1l-2 1.2-14.8 9-2 1.2s3.1 2.2 5 5.1c1.2 1.8 1.8 5 1.8 5v1.7c0 .3-.1.5-.2.6l1.9-1.1.1-.1c.2-.1.3-.3.3-.6v-1.7l14.8-9z"/>
      <path class="st214" d="M-10.2 1751v-1.7l-14.8 9v1.7l9-5.5z"/>
      <path class="st212" d="M-36 1732.3l5.4 3.2c1.1.7 2 2.3 2 3.6v4.5l-1 .6v-4.5c0-1.3-.9-2.9-2-3.6l-6.6-3.5c.3-.3 1-.8 2.2-.3z"/>
      <path class="st159" d="M-36.6 1733.1l5 3.1c1.1.7 2 2.3 2 3.6v4.5l-10-5.9c-.1-7.9 2.3-5.6 3-5.3z"/>
      <path class="st159" d="M-53.1 1741.7l14.7-9 6.8 3.5c1.1.7 2 2.3 2 3.6v4.5l-14.8 9v-4.5c0-1.3-.9-2.9-2-3.6l-6.7-3.5c0-.1 0-.1 0 0z"/>
      <path class="st212" d="M-35.1 1732.8l4.5 2.8c1.1.7 2 2.3 2 3.6v4.5l-1 .6v-4.5c0-1.3-.9-2.9-2-3.6l-6-3.6c.8.2 1.7.5 2.5.2zm-16.7 9l5.4 3.3c1.1.7 2 2.3 2 3.6v4.5l-1 .6v-4.5c0-1.3-.9-2.9-2-3.6l-6.8-3.5c.3-.2 1.2-.8 2.4-.4z"/>
      <path class="st217" d="M-52.4 1742.6l5 3.1c1.1.7 2 2.3 2 3.6v4.5l-10-5.9c0-7.9 2.3-5.5 3-5.3z"/>
      <g id="XMLID_23_">
        <path class="st159" d="M-55.3 1717.2v3.1c0 1 .7 2.2 1.5 2.7l5.9 3.6c.4.2.7.3 1 .1h.1l.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1-.2h-.1c-.3.2-.4.6-.4 1zm1 3.8v-3.1c0-.3.2-.4.4-.3.2.1.4.3.5.4 2.4 1.8 4.5 4.2 5.4 6.3.2.4.3.7.4 1.1v.2c-.1.1-.2.1-.3 0l-5.9-3.6c-.3-.3-.5-.7-.5-1z"/>
        <path class="st218" d="M-54 1715.7l-.9.5c.3-.1.6-.1 1 .2 3.5 2.4 6.4 6 7.2 9 .1.5.1.9-.1 1.2l-.1.1.9-.5.1-.1s.1 0 .1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1.1-.1z"/>
        <path class="st214" d="M-54.3 1719.8v1.2c0 .3.2.7.5.9l5.9 3.6c.2.1.3.1.3 0v-.2c-.1-.3-.2-.7-.4-1.1l-4.9-3c-.3-.2-.5-.6-.5-.9v-2.4c-.2-.1-.4-.3-.5-.4-.2-.1-.4 0-.4.3v2z"/>
      </g>
      <g id="XMLID_22_">
        <path class="st219" d="M-71.1 1718.3c-.1.1-.2.2-.1.5l1.2 6.2c.1.4.3.7.6.8l.6.2h.4c.1-.1.1-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2c-.3-.1-.4-.1-.4 0z"/>
        <path class="st226" d="M-71.1 1718.3h.2l.6.2c.3.1.5.4.6.8l1.2 6.2c0 .2 0 .4-.1.5l.2-.1 2.5-1.5.5-.3 3.7-2.2c.1-.1.2-.2.1-.5l-.1-.3c-.2-.1-.5-.4-.5-.8l-1.1-5.9h-.1l-.6-.2h-.2l-6.9 4.1z"/>
        <path class="st219" d="M-69.2 1730v.9c0 .4.3.9.6 1.1l7.9 4.8c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.2-.2.3-.2.5z"/>
        <path class="st226" d="M-69 1729.6c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l6.8-4.1c.1-.1.2-.2.2-.4v-.5l-7.5-4.5c-.3-.2-.6-.7-.6-1.1v-.5l-.4-.2c-.1-.1-.2-.1-.3-.1h-.1l-2.5 1.5-.4.3-2.5 1.5-.4.3-1.1.5z"/>
        <path class="st92" d="M-68.9 1725.9l.2 1.4c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.2.1h-.1c0 .1-.1.1-.2 0zm3-1.6l.2 1.2c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.5.3z"/>
        <path class="st222" d="M-63.2 1713.5c-.1.1-.2.2-.1.5l.1.3c.2.1.5.4.5.8l1.1 5.9h.1l.6.2h.4c.1-.1.1-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.4z"/>
        <path class="st226" d="M-63.3 1714.3l1.1 5.9c.1.3.3.7.5.8l-1.1-5.9c0-.4-.3-.7-.5-.8zm.1-.8h.2l.6.2c.3.1.5.4.6.8l1.2 6.2c0 .2 0 .4-.1.5l.2-.1 2.5-1.5.5-.3 3.7-2.2c.1-.1.2-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.2l-6.9 4.1zm1.9 12.2v.5c0 .4.3.9.6 1.1l7.5 4.5v-.5c0-.4-.3-.9-.6-1.1l-7.5-4.5z"/>
        <path class="st222" d="M-61.3 1725.2v.5l7.5 4.5c.3.2.6.7.6 1.1v.5l.4.2c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.2-.2.3-.2.5z"/>
        <path class="st226" d="M-61.1 1724.8c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l6.8-4.1c.1-.1.2-.2.2-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.1-.1-.2-.1-.3-.1h-.1l-2.5 1.5-.4.3-2.5 1.5-.4.3-1.1.5z"/>
        <path class="st92" d="M-61 1721.1l.2 1.4c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.2.1h-.1c0 .1-.1.1-.2 0zm2.9-1.6l.2 1.2c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.5.3z"/>
      </g>
      <g id="XMLID_21_">
        <path class="st223" d="M-71.1 1726.8v3.1c0 1 .7 2.2 1.5 2.7l5.9 3.6c.4.2.7.3 1 .1 0 0 .1 0 .1-.1l.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1-.2h-.1c-.3.3-.4.6-.4 1.1zm1 3.7v-3.1c0-.3.2-.4.4-.3.2.1.4.3.5.4 2.4 1.8 4.5 4.2 5.4 6.3.2.4.3.7.4 1.1v.2c-.1.1-.2.1-.3 0l-5.9-3.6c-.3-.3-.5-.7-.5-1z"/>
        <path class="st218" d="M-69.7 1725.2l-.9.5c.3-.1.6-.1 1 .2 3.5 2.4 6.4 6 7.2 9 .1.5.1.9-.1 1.2l-.1.1.9-.5.1-.1.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.5-.2-.9-.3-1.1-.1z"/>
        <path class="st214" d="M-70.1 1729.3v1.2c0 .3.2.7.5.9l5.9 3.6c.2.1.3.1.3 0v-.2c-.1-.3-.2-.7-.4-1.1l-4.9-3c-.3-.2-.5-.6-.5-.9v-2.4c-.2-.1-.4-.3-.5-.4-.2-.1-.4 0-.4.3v2z"/>
      </g>
      <g id="XMLID_20_">
        <path class="st159" d="M-37.5 1727.9v3.1c0 1 .7 2.2 1.5 2.7l5.9 3.6c.4.2.7.3 1 .1 0 0 .1 0 .1-.1l.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1-.2h-.1c-.3.3-.4.6-.4 1.1zm.9 3.7v-3.1c0-.3.2-.4.4-.3.2.1.4.3.5.4 2.4 1.8 4.5 4.2 5.4 6.3.2.4.3.7.4 1.1v.2c-.1.1-.2.1-.3 0l-5.9-3.6c-.2-.3-.5-.7-.5-1z"/>
        <path class="st218" d="M-36.2 1726.3l-.9.5c.3-.1.6-.1 1 .2 3.5 2.4 6.4 6 7.2 9 .1.5.1.9-.1 1.2l-.1.1.9-.5.1-.1s.1 0 .1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.2-.8-.3-1.1-.1z"/>
        <path class="st214" d="M-36.6 1730.4v1.2c0 .3.2.7.5.9l5.9 3.6c.2.1.3.1.3 0v-.2c-.1-.3-.2-.7-.4-1.1l-4.9-3c-.3-.2-.5-.6-.5-.9v-2.4c-.2-.1-.4-.3-.5-.4-.2-.1-.4 0-.4.3v2z"/>
      </g>
      <g id="XMLID_19_">
        <path class="st219" d="M-53.3 1728.9c-.1.1-.2.2-.1.5l1.2 6.2c.1.4.3.7.6.8l.6.2h.4c.1-.1.1-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.4z"/>
        <path class="st227" d="M-53.3 1728.9h.2l.6.2c.3.1.5.4.6.8l1.2 6.2c0 .2 0 .4-.1.5l.2-.1 2.5-1.5.5-.3 3.7-2.2c.1-.1.2-.2.1-.5l-.1-.3c-.2-.1-.5-.4-.5-.8l-1.1-5.9h-.1l-.6-.2h-.2l-6.9 4.1z"/>
        <path class="st219" d="M-51.4 1740.7v.9c0 .4.3.9.6 1.1l7.9 4.8c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.1-.2.3-.2.5z"/>
        <path class="st226" d="M-51.2 1740.2c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l6.8-4.1c.1-.1.2-.2.2-.4v-.5l-7.5-4.5c-.3-.2-.6-.7-.6-1.1v-.5l-.4-.2c-.1-.1-.2-.1-.3-.1h-.1l-2.5 1.5-.4.3-2.5 1.5-.4.3-1.1.5z"/>
        <path class="st92" d="M-51.2 1736.6l.2 1.4c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.2.1h-.3zm3-1.7l.2 1.2c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.5.3z"/>
        <path class="st222" d="M-45.4 1724.1c-.1.1-.2.2-.1.5l.1.3c.2.1.5.4.5.8l1.1 5.9h.1l.6.2h.4c.1-.1.1-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.4z"/>
        <path class="st226" d="M-45.5 1724.9l1.1 5.9c.1.3.3.7.5.8l-1.1-5.9c-.1-.3-.3-.7-.5-.8zm.1-.8h.2l.6.2c.3.1.5.4.6.8l1.2 6.2c0 .2 0 .4-.1.5l.2-.1 2.5-1.5.5-.3 3.7-2.2c.1-.1.2-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.2l-6.9 4.1zm1.9 12.3v.5c0 .4.3.9.6 1.1l7.5 4.5v-.5c0-.4-.3-.9-.6-1.1l-7.5-4.5z"/>
        <path class="st222" d="M-43.5 1735.9v.5l7.5 4.5c.3.2.6.7.6 1.1v.5l.4.2c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.1-.2.3-.2.5z"/>
        <path class="st226" d="M-43.3 1735.5c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l6.8-4.1c.1-.1.2-.2.2-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.1-.1-.2-.1-.3-.1h-.1l-2.5 1.5-.4.3-2.5 1.5-.4.3-1.1.5z"/>
        <path class="st92" d="M-43.3 1731.8l.2 1.4c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.2.1h-.3zm3-1.7l.2 1.2c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.5.3z"/>
      </g>
      <g id="XMLID_15_">
        <path class="st223" d="M-53.3 1737.4v3.1c0 1 .7 2.2 1.5 2.7l5.9 3.6c.4.2.7.3 1 .1 0 0 .1 0 .1-.1l.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1-.2h-.1c-.3.3-.4.7-.4 1.1zm1 3.8v-3.1c0-.3.2-.4.4-.3.2.1.4.3.5.4 2.4 1.8 4.5 4.2 5.4 6.3.2.4.3.7.4 1.1v.2c-.1.1-.2.1-.3 0l-5.9-3.6c-.3-.3-.5-.7-.5-1z"/>
        <path class="st218" d="M-52 1735.9l-.9.5c.3-.1.6-.1 1 .2 3.5 2.4 6.4 6 7.2 9 .1.5.1.9-.1 1.2l-.1.1.9-.5.1-.1.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1.1-.1z"/>
        <path class="st214" d="M-52.3 1740v1.2c0 .3.2.7.5.9l5.9 3.6c.2.1.3.1.3 0v-.2c-.1-.3-.2-.7-.4-1.1l-4.9-3c-.3-.2-.5-.6-.5-.9v-2.4c-.2-.1-.4-.3-.5-.4-.2-.1-.4 0-.4.3v2z"/>
      </g>
      <path class="st214" d="M-29.8 1743.7c.2-.1.4-.1.7.1l.7.4-1.5.9-2.4 1.5-.7-.4c-.3-.2-.5-.2-.7-.1l3.9-2.4z"/>
      <path class="st92" d="M-34.1 1746.7c0 .2.1.5.2.7l1.5-.9-.7-.4c-.3-.2-.5-.2-.7-.1-.1.1-.3.4-.3.7zm1.8-.9s.2.2.6-.1c.2-.1 0-.3 0-.3l-7.1-11.5-.6.4 7.1 11.5z"/>
      <path class="st92" d="M-42.3 1736.6c.1 0 .3-.1.5-.2h.1c.3-.1.8-.5 1.1-.6h.1c.4-.2 1.2-.7 1.6-1 .4-.3 1.2-.8 1.7-1.1l.1-.1c.3-.2.9-.6 1.1-.9l.1-.1c.3-.2.6-.5.4-.8-.1-.1-.2-.2-.3-.2-.1 0-.3.1-.5.2h-.1c-.3.1-.8.5-1.1.6h-.1c-.4.2-1.2.8-1.6 1-.4.3-1.3.8-1.7 1.1l-.1.1c-.3.2-.9.6-1.1.9l-.1.1c-.3.3-.6.5-.4.8 0 .1.1.2.3.2z"/>
      <g id="XMLID_2_">
        <path class="st228" d="M-31.2 1747.2l.3 1.4 14.5-8.8-.7-.6-.1-.5z"/>
        <path class="st216" d="M-30.9 1748.6l.1.4 14.8-8.9.2-.7z"/>
        <path class="st228" d="M-17.2 1738.7l.1.5.7.6.3-.2z"/>
      </g>
      <path class="st216" d="M-15 1739.4c0-.1-.3-5.2-.8-8.8-.6-4.9-3.8-9.4-6.5-11.3-4.9-3.6-41.7-24-41.9-24l-1.3-.8c-.9-.4-2.7-1.1-4.9.2-1.4.9-2.2 2.6-2.6 4.9l.9.1c.3-1.9 1-3.3 2-4 1.5-.9 3.8-.1 4.1.1 1.1.6 38.5 22.1 42.6 24.7 5.8 3.6 7 19.7 7 19.7l1.4-.8z"/>
      <path class="st215" d="M-16.2 1739.6c0-.4-.3-5.4-.8-9.1-.6-4.8-4-9.6-6.8-11.2-4.2-2.4-42.5-24-42.7-24.1-.1-.1-2.4-1.3-4.3-.1-1.3.8-2.1 3-2.2 5.4l1.2.5c.1-1.9.8-4.2 1.7-4.7 1.2-.7 2.9.1 3.1.2.7.4 36.7 21.5 41.1 23.3 9 3.6 8.7 18.9 8.7 19.1l1 .7z"/>
      <path class="st216" d="M-30.6 1748.9c0-.1.3-2.4-.2-6-.6-4.9-3.5-12.3-6.9-14.2-5.3-2.9-41.9-24-42.1-24l-1.3-.8c-.9-.4-2-1.4-5.6.6-1.5.8-3.4 20.5-3.7 22.8l.9-.5c.9-5.8 2.4-19.5 3.6-20.9 1.2-1.4 3-.2 3.3-.1 1.1.6 39.7 21.6 43.9 24.2 5.8 3.6 6.8 19.7 6.8 19.7l1.3-.8z"/>
      <path class="st216" d="M-73.8 1710.8c-1.8-1.1-3.9-1.8-5.6-3.1-1.6-1.3-3.6-2.5-5.6-2.7-.4 0-.6.1-.8.3-.7-.4-.8-.8-.8-.8l16.3-9.8 2.9-.7c.7.4 40.3 22.9 44.7 25.6 0 0 2.8 2.3 3.3 3.5l-16.9 8.6.1.5c-.7-.7-1.6-2.4-2.5-2.9-.8-.4-20.7-10.5-34.7-17.7.1-.3-.1-.6-.4-.8z"/>
      <path class="st229" d="M-20 1723.1s-9.3 3.2-15.3 8c0 0 .6.6 1 1.4 0 0 6.6-5.1 15.2-7.9.1 0-.3-.9-.9-1.5z"/>
      <linearGradient id="SVGID_10_" gradientUnits="userSpaceOnUse" x1="6148.919" y1="1724.616" x2="6148.919" y2="1748.292" gradientTransform="matrix(-.477 0 0 1 2906.666 0)">
        <stop offset="0" stop-color="#FFF" stop-opacity="0"/>
        <stop offset="1" stop-opacity=".4"/>
      </linearGradient>
      <path class="st241" d="M-16.2 1739.6s-.5-12.4-2.9-15c0 0-9.1 2.8-15.2 7.9 0 0 3.9 5.6 3.7 15.7l14.4-8.6z"/>
      <path class="st215" d="M-31.8 1749.6c-.1.7.3-3.1-.2-6.9-.6-4.8-3.4-11.9-7.1-14-4.2-2.4-42.7-24-42.9-24.1-.1-.1-2.4-1.3-4.3-.1-1.3.8-1.9 2.7-2.1 5.7l.9.3c.6-3.8 1-4.3 1.8-4.9 1.2-.7 2.9.2 3.1.3.7.4 38.6 21.9 42.9 24.1 7 3.8 7 18.7 7 18.8l.9.8z"/>
      <path class="st215" d="M-87.5 1709.9h-1l-2.5 16.8.7.6z"/>
    </g>
    <g id="golf-kart-3">
      <path class="st211" d="M913.5 3485.5l16.7-10.1 6.6 4-1.9 1.2-16.8 10.1-4.6-2.8-2-1.2z"/>
      <g id="XMLID_48_">
        <path class="st212" d="M921.1 3484.4c-.1.1-.1.1-.1.2.2 0 .5.1.8.3l7.6 4.6 11.7 7.1c1.1.7 2 2.3 2 3.6v4.5l1-.6v-4.5c0-1.3-.9-2.9-2-3.6l-19.4-11.7c-.3-.2-.6-.3-.8-.3-.3 0-.6.2-.8.4z"/>
        <path class="st159" d="M921.9 3484c.2 0 .5.1.8.3l19.4 11.7c1.1.7 2 2.3 2 3.6v4.5l14.8-9v-4.5c0-1.3-.9-2.9-2-3.6l-11.7-7.1-7.6-4.6c-.3-.2-.5-.3-.8-.3l-14.9 9z"/>
        <path class="st212" d="M936.9 3474.9c-.1.1-.1.1-.1.2.2 0 .5.1.8.3l7.6 4.6 11.7 7.1c1.1.7 2 2.3 2 3.6v4.5l1-.6v-4.5c0-1.3-.9-2.9-2-3.6l-19.4-11.7c-.7-.5-1.2-.4-1.6.1z"/>
      </g>
      <g id="XMLID_47_">
        <path class="st159" d="M947.2 3461.7v19.5l1.1.6v-19.5z"/>
        <path class="st213" d="M947.2 3461.7l1.1.6 1-.6-1.1-.6zm1.1.6v19.5l1-.6v-19.5z"/>
      </g>
      <g id="XMLID_46_">
        <path class="st159" d="M987.3 3514.8c0 2.6 1.8 5.8 3.9 7.1 1.1.7 2.1.7 2.8.3.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3-.6.4-1.1 1.3-1.1 2.6zm4 5.4c-1.4-.8-2.5-2.8-2.5-4.5 0-1.1.5-1.8 1.3-1.8.4 0 .8.1 1.2.4 1.4.8 2.5 2.8 2.5 4.5 0 .5-.1.9-.3 1.2-.5.6-1.3.8-2.2.2z"/>
        <path class="st214" d="M991.5 3510.4l-3 1.8c.7-.4 1.7-.3 2.8.3 2.2 1.3 3.9 4.5 3.9 7.1 0 1.3-.4 2.2-1.1 2.6l3-1.8c.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.7-2.1-.7-2.8-.3z"/>
        <path class="st214" d="M988.8 3515.7c0 1.6 1.1 3.6 2.5 4.5.9.6 1.8.4 2.2-.2-.4 0-.8-.1-1.2-.3-1.4-.8-2.5-2.8-2.5-4.5 0-.5.1-.9.3-1.2-.8-.1-1.3.6-1.3 1.7z"/>
        <path class="st92" d="M990.1 3513.9c-.2.3-.3.7-.3 1.2 0 1.6 1.1 3.6 2.5 4.5.4.3.8.4 1.2.3.2-.3.3-.7.3-1.2 0-1.6-1.1-3.6-2.5-4.5-.5-.2-.9-.3-1.2-.3z"/>
      </g>
      <g id="XMLID_45_">
        <path class="st215" d="M929.8 3471.4l-.9 6 .8.6.9-6c.2-1.3.9-2.2 1.8-2.4.5-.1 1.1 0 1.7.3l3 1.9v1.9c0 .8.5 1.7 1.1 2.1l4.5 2.8c.3.2.6.2.8.1 0 0 .1 0 .1-.1.2-.2.2-.5.1-.9-.6-2.3-2.8-5.1-5.5-6.9-.3-.2-.6-.3-.8-.1h-.1c-.1.1-.2.2-.2.3l-3-1.9c-.8-.5-1.6-.6-2.2-.4-.2 0-.3.1-.4.2l-.1.1c-.8.3-1.4 1.2-1.6 2.4zm8.1 2.8v-2.4c0-.2.1-.3.3-.2.2.1.4.3.6.5 1.6 1.2 3 2.8 3.7 4.3.2.4.4.8.5 1.2v.1s-.1.1-.3 0l-4.5-2.8c-.2-.2-.3-.5-.3-.7z"/>
        <path class="st216" d="M930.6 3472l-.9 6 1-.6.9-6c.1-.8.4-1.4.8-1.8-.9.2-1.6 1.1-1.8 2.4z"/>
        <path class="st217" d="M932.2 3468.3l-.8.5c.1-.1.3-.1.4-.2.7-.2 1.5-.1 2.2.4l3 1.9c.1-.1.1-.2.2-.3h.1l.6-.3-2.9-1.8c-1-.6-1.9-.6-2.7-.2h-.1z"/>
        <path class="st218" d="M938.4 3470l-.3.2-.6.3c.2-.1.5-.1.8.1 2.7 1.9 4.9 4.7 5.5 6.9.1.4.1.7-.1.9 0 0 0 .1-.1.1l.9-.6.1-.1c.2-.2.2-.5.1-.9-.6-2.3-2.8-5.1-5.5-6.9-.3-.2-.6-.2-.8 0z"/>
        <path class="st214" d="M937.9 3471.8v2.4c0 .3.2.6.4.7l4.5 2.8c.1.1.2.1.3 0v-.1c-.1-.4-.3-.8-.5-1.2l-3.3-2c-.2-.1-.4-.4-.4-.7v-1.6c-.2-.2-.4-.3-.6-.5-.3-.2-.4-.1-.4.2z"/>
      </g>
      <g id="XMLID_44_">
        <path class="st219" d="M921.6 3481.9v.9c0 .4.3.9.6 1.1l7.9 4.8c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.2.2-.2.3-.2.5z"/>
        <path class="st220" d="M921.7 3481.5c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l2.6-1.6-.2-.3c-.1.1-.2.1-.3.1v-.6c.1 0 .2-.1.2-.3l.6-2.7-2.8 1.7-.1.1c-.1 0-.3 0-.4-.2l-.6-.6c-.3-.2-.4-.7-.4-.9l1.1-4.3h-.1c-.3-.2-.6-.7-.6-1.1v-.5l-.4-.2c-.2-.1-.3-.1-.4 0l-7 4.1z"/>
        <path class="st219" d="M929.1 3483.5c-.1.3.1.7.4.9l.6.6c.1.1.3.2.4.2l.1-.1.1-.1 1.2-4.7-1.7-1-1.1 4.2z"/>
        <path class="st220" d="M929.5 3477.6v.5c0 .4.3.9.6 1.1h.1l.3-1-1-.6z"/>
        <path class="st221" d="M929.5 3477.1v.5l.9.6.3-1-.6-.3c-.2-.1-.3-.1-.4-.1-.2 0-.2.1-.2.3z"/>
        <path class="st220" d="M929.6 3476.7c.1 0 .3 0 .4.1l.6.3.1-.2c0-.1 0-.1.1-.2l.1-.1 6.4-3.9-.3-.2c-.2-.1-.3-.1-.4 0l-7 4.2z"/>
        <path class="st219" d="M930.4 3478.2l-.3 1 1.7 1 .3-1zm.2-1.1l-.3 1 1.7 1 .2-.9v-.2l-1.6-.9z"/>
        <path class="st222" d="M930.6 3485.1l2.8-1.7.1-.5c.1-.3 0-.9-.2-1.3l-.1-.1.1-.4-1.5-.9-1.2 4.7v.2z"/>
        <path class="st219" d="M930.7 3476.9l-.1.2 1.7 1c0-.3-.2-.5-.4-.7l-.6-.6c-.1-.1-.3-.2-.4-.2l-.1.1c-.1.1-.1.1-.1.2z"/>
        <path class="st222" d="M937.3 3472.8l-6.4 3.9c.1 0 .3 0 .4.2l.6.6c.2.2.3.5.4.7l4.2 2.5c0-.3-.1-.6-.3-.8l-.1-.1.1-.5.2.5c.2.4.3.8.4 1.2l.3.2.3-.2.1-.1.2-.7-.4-.4c-.3-.2-.4-.7-.4-.9l1.3-5.3-.9-.8zm-5.2 6.4l-.3 1 1.5.9v-.1l.1.2 1.8 1.1 1-.6z"/>
        <path class="st222" d="M932.1 3479.2l4.1 2.5.2-.1.1-.5v-.4l-4.2-2.5v.2l-.2.8z"/>
        <path class="st92" d="M932.6 3486.3v.6c.1 0 .2 0 .3-.1.1-.1.2-.2.3-.4l.7-3.2v-.2l-.5.3-.6 2.7c0 .2-.1.3-.2.3z"/>
        <path class="st220" d="M932.9 3486.8l.2.3 4.2-2.6c.1-.1.2-.2.2-.4v-.5l-1-.6-.3 1.6c-.1.3-.3.5-.6.5v-.6c.1 0 .2-.1.2-.3l.3-1.5-.9-.5-1.3.8v.2l-.7 3.2c0 .2-.1.4-.3.4z"/>
        <path class="st92" d="M933.3 3481.1l-.1.4.1.1c.2.4.3 1 .2 1.3l-.1.5.5-.3c0-.5-.1-1.1-.4-1.6l-.1-.3-.1-.1z"/>
        <path class="st92" d="M933.3 3481v.1l.1.1z"/>
        <path class="st222" d="M933.4 3481.2l.1.3c.3.5.4 1.1.4 1.6l1.3-.8-1.8-1.1z"/>
        <path class="st220" d="M935.2 3482.3l.9.5.2-1-.1-.1z"/>
        <path class="st92" d="M935.5 3484.6v.6c.3 0 .5-.2.6-.5l.3-1.6-.4-.2-.3 1.5s0 .1-.2.2zm.8-2.8l-.2 1 .4.2.2-1zm0-2.6l-.1.5.1.1c.1.2.2.6.3.8l.4.2c0-.4-.2-.9-.4-1.2l-.3-.4z"/>
        <path class="st222" d="M936.2 3481.7l.1.1v-.2z"/>
        <path class="st92" d="M936.3 3481.6v.2l.4.2.1-.6v-.2l-.5.4z"/>
        <path class="st92" d="M936.5 3481.1l-.1.5.5-.3v-.4l-.4-.2v.4z"/>
        <path class="st220" d="M936.7 3482l-.2 1 1 .6v-.5c0-.4-.3-.9-.6-1.1h-.2z"/>
        <path class="st221" d="M936.8 3481.4l-.1.6.2.1c.3.2.6.7.6 1.1v.5l.4.2c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-.7-.4-.3.2s0 .1-.1.1z"/>
        <path class="st222" d="M937.2 3481.1l-.3-.2v.4l.3-.2zm-.2-2.4c-.1.3.1.7.4.9l.4.4 1.4-5.9v-.2l-.9-.6-1.3 5.4z"/>
        <path class="st220" d="M937.2 3481.1l.7.4c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l2.6-1.6-.2-.3c-.1.1-.2.1-.3.1v-.6c.1 0 .2-.1.2-.3l.6-2.7-2.8 1.7-.1.1c-.1 0-.3 0-.4-.2l-.2-.2-.2.7c0 .1 0 .1-.1.1l-.3.4z"/>
        <path class="st222" d="M937.7 3472.5l-.4.2 1 .6.1-.6-.2-.2c-.2-.1-.3-.2-.4-.2l-.1.2z"/>
        <path class="st219" d="M939.2 3474.1l-1.4 5.9.2.2c.1.1.3.2.4.2l.1-.1.1-.1 1.4-5.7-.8-.5v.1z"/>
        <path class="st222" d="M938.4 3472.8l-.1.6.9.6c0-.3-.2-.5-.4-.7l-.4-.5z"/>
        <path class="st219" d="M938.6 3472.1l-.2.7.4.4c.2.2.3.5.4.7l.8.5.2-.9c.1-.3-.1-.7-.4-.9l-.6-.6c-.1-.1-.3-.2-.4-.2l-.1.1c-.1.1-.1.1-.1.2z"/>
        <path class="st222" d="M938.5 3480.3l2.8-1.7.1-.5c.1-.3 0-.9-.2-1.3l-.1-.1.1-.5.2.5c.3.5.4 1.1.4 1.6l2.3-1.4-4.1-2.5-1.4 5.7c-.1.1-.1.2-.1.2z"/>
        <path class="st222" d="M945.6 3467.8l-6.8 4.1c.1 0 .3 0 .4.2l.6.6c.3.2.4.7.4.9l-.2.9 4.1 2.5.2-.1.1-.5c.1-.3 0-.9-.2-1.3l-.1-.1.1-.5.2.5c.3.5.4 1.1.4 1.6l.6-.4.1-.1 1.6-6.6c.1-.3-.1-.7-.4-.9l-.6-.6c-.2-.1-.3-.2-.4-.2h-.1z"/>
        <path class="st92" d="M940.5 3481.6v.6c.1 0 .2 0 .3-.1.1-.1.2-.2.3-.4l.7-3.2v-.2l-.5.3-.6 2.7c0 .1-.1.2-.2.3z"/>
        <path class="st220" d="M940.8 3482.1l.2.3 4.2-2.6c.1-.1.2-.2.2-.4v-1c0-.4-.3-.9-.6-1.1l-.2-.1-.6 2.6c-.1.3-.3.5-.6.5v-.6c.1 0 .2-.1.2-.3l.5-2.5-.1-.1-2.3 1.4v.2l-.7 3.2c0 .2-.1.4-.2.5z"/>
        <path class="st92" d="M941.2 3476.2l-.1.5.1.1c.2.4.3 1 .2 1.3l-.1.5.5-.3c0-.5-.1-1.1-.4-1.6l-.2-.5zm2.2 3.6v.6c.3 0 .5-.2.6-.5l.6-2.6-.4-.2-.5 2.5c-.1 0-.2.1-.3.2zm.7-5.4l-.1.5.1.1c.2.4.3 1 .2 1.3l-.1.5.5-.3c0-.5-.1-1.1-.4-1.6l-.2-.5z"/>
        <path class="st92" d="M944.2 3476.8v.2l.4.2.1-.6v-.2l-.5.4z"/>
      </g>
      <path class="st217" d="M920.8 3484.6c-.2 0-.5.2-.6.4l7.3 4.4c3.1 1.8 5.6 5.8 6.5 9.7l9.1 5.5v-4.5c0-1.3-.9-2.9-2-3.6l-11.7-7.1-7.6-4.6c-.3-.2-.5-.3-.8-.3-.1.1-.2.1-.2.1z"/>
      <path class="st212" d="M919.2 3485.6l7.3 4.4c3.1 1.8 5.6 5.8 6.5 9.7l1-.6c-.9-3.9-3.4-7.8-6.5-9.7l-7.3-4.4-1 .6z"/>
      <path class="st214" d="M921.6 3492.8c-.2.6-.4 1.3-.4 2.2l2-1.2c0-1.2.3-2.1.7-2.7-1.1 0-1.9.7-2.3 1.7z"/>
      <path class="st214" d="M921.2 3495c0-.8.1-1.6.4-2.2l-1.5-.9-2-1.2-4.6-2.8-2-1.2v2.4l6.6 4 3.1 1.9z"/>
      <path class="st92" d="M923.1 3493.8l8.3 5c-.8-2.8-2.7-5.7-4.9-7-1-.6-1.9-.8-2.7-.8-.4.7-.7 1.6-.7 2.8zm56.1 26.4c0 .3-.1.5-.2.6h-.1l-1.9 1.1h-.1c-.2.1-.4.1-.7-.1l-1.7-1.1c-1-.6-1.9-.8-2.7-.8-.4.7-.7 1.6-.7 2.7l8.9 3.1c1.1.4 1.6-.5 1.1-2l-.7-2.5c-.1-.4-.5-.9-.7-1.1-.3.3-.5.1-.5.1z"/>
      <path class="st212" d="M933 3499.7l24.8 15.1 6.2 3.7c1.1.7 2.4.6 3-.2l.5-.6c-.5 0-1-.2-1.5-.5l-21.8-13.3-1 .6-9.1-5.5-1.1.7z"/>
      <path class="st214" d="M971.9 3520.2c-1.6.1-2.7 1.6-2.7 3.9l2-1.2c0-1.1.2-2 .7-2.7z"/>
      <g id="XMLID_43_">
        <path class="st159" d="M921.6 3496.4c0 2.6 1.8 5.8 3.9 7.1 1.1.7 2.1.7 2.8.3.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3-.7.4-1.1 1.3-1.1 2.6zm3.9 5.4c-1.4-.8-2.5-2.8-2.5-4.5 0-1.1.5-1.8 1.3-1.8.4 0 .8.1 1.2.4 1.4.8 2.5 2.8 2.5 4.5 0 .5-.1.9-.3 1.2-.4.6-1.2.7-2.2.2z"/>
        <path class="st214" d="M931.3 3502c.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3l-3 1.8c.7-.4 1.7-.3 2.8.3 2.2 1.3 3.9 4.5 3.9 7.1 0 1.3-.4 2.2-1.1 2.6l3-1.8z"/>
        <path class="st218" d="M923 3497.3c0 1.6 1.1 3.6 2.5 4.5.9.6 1.8.4 2.2-.2-.4 0-.8-.1-1.2-.3-1.4-.8-2.5-2.8-2.5-4.5 0-.5.1-.9.3-1.2-.7-.1-1.3.6-1.3 1.7z"/>
        <path class="st223" d="M924.3 3495.5c-.2.3-.3.7-.3 1.2 0 1.6 1.1 3.6 2.5 4.5.4.3.8.4 1.2.3.2-.3.3-.7.3-1.2 0-1.6-1.1-3.6-2.5-4.5-.4-.2-.8-.3-1.2-.3z"/>
      </g>
      <g id="XMLID_42_">
        <path class="st159" d="M969.6 3525.6c0 2.6 1.8 5.8 3.9 7.1 1.1.7 2.1.7 2.8.3.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3-.7.3-1.1 1.2-1.1 2.6zm3.9 5.3c-1.4-.8-2.5-2.8-2.5-4.5 0-1.1.5-1.8 1.3-1.8.4 0 .8.1 1.2.4 1.4.8 2.5 2.8 2.5 4.5 0 .5-.1.9-.3 1.2-.4.7-1.2.8-2.2.2z"/>
        <path class="st214" d="M979.3 3531.2c.7-.4 1.1-1.3 1.1-2.6 0-2.6-1.8-5.8-3.9-7.1-1.1-.6-2-.7-2.8-.3l-3 1.8c.7-.4 1.7-.3 2.8.3 2.2 1.3 3.9 4.5 3.9 7.1 0 1.3-.4 2.2-1.1 2.6l3-1.8z"/>
        <path class="st218" d="M971.1 3526.5c0 1.6 1.1 3.6 2.5 4.5.9.6 1.8.4 2.2-.2-.4 0-.8-.1-1.2-.3-1.4-.8-2.5-2.8-2.5-4.5 0-.5.1-.9.3-1.2-.8-.1-1.3.5-1.3 1.7z"/>
        <path class="st223" d="M972.3 3524.6c-.2.3-.3.7-.3 1.2 0 1.6 1.1 3.6 2.5 4.5.4.3.8.4 1.2.3.2-.3.3-.7.3-1.2 0-1.6-1.1-3.6-2.5-4.5-.4-.2-.8-.3-1.2-.3z"/>
      </g>
      <path class="st224" d="M919.1 3485.6c-.5.6-.8 1.8-.9 2.8-.2 1.2-.1 2.3-.1 2.3l2 1.2 1.5.9c.4-1.1 1.3-1.7 2.3-1.8.8-.1 1.7.2 2.7.8 2.2 1.4 4.2 4.2 4.9 7 .2.9.4 1.8.4 2.6l37.4 22.7c0-2.4 1.1-3.8 2.7-3.9.8-.1 1.7.2 2.7.8l1.7 1.1c.3.2.5.2.7.1h.1c.2-.1.2-.3.2-.6v-1.7s-1.7-1-3.8-2.3c-2.1-1.3-3.8-2.3-3.8-2.3l-2.1 2.7-.5.6c-.6.7-2 .8-3 .2l-6.2-3.7-24.8-15.1c-.9-3.9-3.4-7.8-6.5-9.7l-7.6-4.7z"/>
      <g id="XMLID_41_">
        <path class="st223" d="M921.3 3481.3v1.9c0 .8.5 1.7 1.1 2.1l4.5 2.8c.3.2.6.2.8.1 0 0 .1 0 .1-.1.2-.2.2-.5.1-.9-.6-2.3-2.8-5.1-5.5-6.9-.3-.2-.6-.3-.8-.1h-.1c-.1.1-.2.2-.2.3m.8 3.2v-2.4c0-.2.1-.3.3-.2.2.1.4.3.6.5 1.6 1.2 3 2.8 3.7 4.3.2.4.4.8.5 1.2v.1s-.1.1-.3 0l-4.5-2.8c-.1-.1-.3-.4-.3-.7z"/>
        <path class="st218" d="M922.6 3479.5l-.3.2-.6.3c.2-.1.5-.1.8.1 2.7 1.9 4.9 4.7 5.5 6.9.1.4.1.7-.1.9l-.1.1.9-.6.1-.1c.2-.2.2-.5.1-.9-.6-2.3-2.8-5.1-5.5-6.9-.3-.1-.6-.1-.8 0z"/>
        <path class="st214" d="M922.1 3481.3v2.4c0 .3.2.6.4.7l4.5 2.8c.1.1.2.1.3 0v-.1c-.1-.4-.3-.8-.5-1.2l-3.3-2c-.2-.1-.4-.4-.4-.7v-1.6c-.2-.2-.4-.3-.6-.5-.3-.1-.4 0-.4.2z"/>
      </g>
      <path class="st212" d="M974.9 3504.9l2-1.2-17.1-9.2-.9.6 16.8 9.3-1.2.3z"/>
      <path class="st223" d="M970.3 3507.7s.1-.1.2-.1l5.2-3.2-16.9-9.4-14.8 8.9 21.8 13.3c.5.3 1 .4 1.5.5l1.7-2.2 1-7.4c.1-.1.2-.3.3-.4z"/>
      <path class="st214" d="M970.1 3508.2l-1 7.4.4-.5.9-5.5 2-1.2-1.2-.7c-.3-.2-.5-.2-.7-.1l-.2.1c-.1.1-.2.3-.2.5z"/>
      <path class="st159" d="M985.1 3498.7l-14.6 8.8c.2-.1.5 0 .7.1l1.2.7 12.3-7.4 2.5-1.5-1.2-.7c-.3-.2-.5-.2-.7-.1l-.2.1z"/>
      <g id="XMLID_40_">
        <path class="st217" d="M931.4 3471.2v19.5l1.1.7v-19.6z"/>
        <path class="st213" d="M931.4 3471.2l1.1.6 1-.6-1.1-.6zm1.1.6v19.6l1-.6v-19.6z"/>
      </g>
      <path class="st224" d="M970.4 3509.6l-.9 5.5s1.7 1 3.8 2.3c2.1 1.3 3.8 2.3 3.8 2.3s-.5-3.2-1.8-5c-1.8-2.9-4.9-5.1-4.9-5.1z"/>
      <path class="st225" d="M988.2 3514.8l4.8-2.9 1-.6.4.2h.1c.3.2.6.6.7 1.1l.7 2.5c.3 1 .2 1.7-.3 2L981 3526c.3-.3.4-1 .2-1.9l-.7-2.5c-.1-.4-.5-.9-.7-1.1-.3-.2-.5-.3-.5-.3l8.9-5.4z"/>
      <path class="st159" d="M994 3509.6v1.7l.4.2 1.2-.7c.2-.1.3-.3.3-.7v-1.7s-.5-3.2-1.8-5c-2-3-5-5.1-5-5.1l-2 1.2-14.8 9-2 1.2s3.1 2.2 5 5.1c1.2 1.8 1.8 5 1.8 5v1.7c0 .3-.1.5-.2.6l1.9-1.1.1-.1c.2-.1.3-.3.3-.6v-1.7l14.8-9z"/>
      <path class="st214" d="M994 3511.3v-1.7l-14.8 8.9v1.7l9-5.4z"/>
      <path class="st212" d="M968.2 3492.6l5.4 3.2c1.1.7 2 2.3 2 3.6v4.5l-1 .6v-4.5c0-1.3-.9-2.9-2-3.6l-6.6-3.5c.2-.3 1-.8 2.2-.3z"/>
      <path class="st159" d="M967.5 3493.4l5 3.1c1.1.7 2 2.3 2 3.6v4.5l-10-5.9c0-8 2.4-5.6 3-5.3z"/>
      <path class="st159" d="M951.1 3501.9l14.7-9 6.8 3.5c1.1.7 2 2.3 2 3.6v4.5l-14.8 9v-4.5c0-1.3-.9-2.9-2-3.6l-6.7-3.5z"/>
      <path class="st212" d="M969.1 3493.1l4.5 2.8c1.1.7 2 2.3 2 3.6v4.5l-1 .6v-4.5c0-1.3-.9-2.9-2-3.6l-6-3.6c.8.2 1.7.5 2.5.2zm-16.7 9l5.4 3.3c1.1.7 2 2.3 2 3.6v4.5l-1 .6v-4.5c0-1.3-.9-2.9-2-3.6l-6.8-3.5c.3-.2 1.2-.9 2.4-.4z"/>
      <path class="st217" d="M951.8 3502.9l5 3.1c1.1.7 2 2.3 2 3.6v4.5l-10-5.9c-.1-7.9 2.3-5.5 3-5.3z"/>
      <g id="XMLID_39_">
        <path class="st159" d="M948.8 3477.5v3.1c0 1 .7 2.2 1.5 2.7l5.9 3.6c.4.2.7.3 1 .1 0 0 .1 0 .1-.1l.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1-.2h-.1c-.2.3-.4.6-.4 1.1zm1 3.7v-3.1c0-.3.2-.4.4-.3.2.1.4.3.5.4 2.4 1.8 4.5 4.2 5.4 6.3.2.4.3.7.4 1.1v.2c-.1.1-.2.1-.3 0l-5.9-3.6c-.3-.2-.5-.6-.5-1z"/>
        <path class="st218" d="M950.2 3476l-.9.5c.3-.1.6-.1 1 .2 3.5 2.4 6.4 6 7.2 9 .1.5.1.9-.1 1.2l-.1.1.9-.5.1-.1s.1 0 .1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1.1-.1z"/>
        <path class="st214" d="M949.8 3480v1.2c0 .3.2.7.5.9l5.9 3.6c.2.1.3.1.3 0v-.2c-.1-.3-.2-.7-.4-1.1l-4.9-3c-.3-.2-.5-.6-.5-.9v-2.4c-.2-.1-.4-.3-.5-.4-.2-.1-.4 0-.4.3v2z"/>
      </g>
      <g id="XMLID_38_">
        <path class="st219" d="M933.1 3478.6c-.1.1-.2.2-.1.5l1.2 6.2c.1.4.3.7.6.8l.6.2h.4c.1-.1.1-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2c-.3-.1-.4-.1-.4 0z"/>
        <path class="st226" d="M933.1 3478.5h.2l.6.2c.3.1.5.4.6.8l1.2 6.2c0 .2 0 .4-.1.5l.2-.1 2.5-1.5.5-.3 3.7-2.2c.1-.1.2-.2.1-.5l-.1-.3c-.2-.1-.5-.4-.5-.8l-1.1-5.9h-.1l-.6-.2h-.2l-6.9 4.1z"/>
        <path class="st219" d="M935 3490.3v.9c0 .4.3.9.6 1.1l7.9 4.8c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.1-.2.3-.2.5z"/>
        <path class="st226" d="M935.2 3489.9c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l6.8-4.1c.1-.1.2-.2.2-.4v-.5l-7.5-4.5c-.3-.2-.6-.7-.6-1.1v-.5l-.4-.2c-.1-.1-.2-.1-.3-.1h-.1l-2.5 1.5-.4.3-2.5 1.5-.4.3-1.1.5z"/>
        <path class="st92" d="M935.2 3486.2l.2 1.4c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.2.1h-.3zm3-1.6l.2 1.2c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.5.3z"/>
        <path class="st222" d="M940.9 3473.8c-.1.1-.2.2-.1.5l.1.3c.2.1.5.4.5.8l1.1 5.9h.1l.6.2h.4c.1-.1.1-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2c-.2-.1-.3-.1-.4 0z"/>
        <path class="st226" d="M940.9 3474.6l1.1 5.9c.1.3.3.7.5.8l-1.1-5.9c-.1-.4-.3-.7-.5-.8zm0-.8h.2l.6.2c.3.1.5.4.6.8l1.2 6.2c0 .2 0 .4-.1.5l.2-.1 2.5-1.5.5-.3 3.7-2.2c.1-.1.2-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.2l-6.9 4.1zm2 12.2v.5c0 .4.3.9.6 1.1l7.5 4.5v-.5c0-.4-.3-.9-.6-1.1l-7.5-4.5z"/>
        <path class="st222" d="M942.9 3485.5v.5l7.5 4.5c.3.2.6.7.6 1.1v.5l.4.2c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.2-.2.3-.2.5z"/>
        <path class="st226" d="M943.1 3485.1c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l6.8-4.1c.1-.1.2-.2.2-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.1-.1-.2-.1-.3-.1h-.1l-2.5 1.5-.4.3-2.5 1.5-.4.3-1.1.5z"/>
        <path class="st92" d="M943.1 3481.4l.2 1.4c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.2.1h-.1c0 .1 0 .1-.2 0zm3-1.6l.2 1.2c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.5.3z"/>
      </g>
      <g id="XMLID_37_">
        <path class="st223" d="M933.1 3487.1v3.1c0 1 .7 2.2 1.5 2.7l5.9 3.6c.4.2.7.3 1 .1 0 0 .1 0 .1-.1l.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1-.2h-.1c-.3.3-.4.6-.4 1.1zm1 3.7v-3.1c0-.3.2-.4.4-.3.2.1.4.3.5.4 2.4 1.8 4.5 4.2 5.4 6.3.2.4.3.7.4 1.1v.2c-.1.1-.2.1-.3 0l-5.9-3.6c-.3-.3-.5-.7-.5-1z"/>
        <path class="st218" d="M934.4 3485.5l-.9.5c.3-.1.6-.1 1 .2 3.5 2.4 6.4 6 7.2 9 .1.5.1.9-.1 1.2l-.1.1.9-.5.1-.1.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1.1-.1z"/>
        <path class="st214" d="M934.1 3489.6v1.2c0 .3.2.7.5.9l5.9 3.6c.2.1.3.1.3 0v-.2c-.1-.3-.2-.7-.4-1.1l-4.9-3c-.3-.2-.5-.6-.5-.9v-2.4c-.2-.1-.4-.3-.5-.4-.2-.1-.4 0-.4.3v2z"/>
      </g>
      <g id="XMLID_36_">
        <path class="st159" d="M966.6 3488.2v3.1c0 1 .7 2.2 1.5 2.7l5.9 3.6c.4.2.7.3 1 .1 0 0 .1 0 .1-.1l.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1-.2h-.1c-.2.3-.4.6-.4 1.1zm1 3.7v-3.1c0-.3.2-.4.4-.3.2.1.4.3.5.4 2.4 1.8 4.5 4.2 5.4 6.3.2.4.3.7.4 1.1v.2c-.1.1-.2.1-.3 0l-5.9-3.6c-.3-.3-.5-.7-.5-1z"/>
        <path class="st218" d="M968 3486.6l-.9.5c.3-.1.6-.1 1 .2 3.5 2.4 6.4 6 7.2 9 .1.5.1.9-.1 1.2l-.1.1.9-.5.1-.1.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1.1-.1z"/>
        <path class="st214" d="M967.6 3490.7v1.2c0 .3.2.7.5.9l5.9 3.6c.2.1.3.1.3 0v-.2c-.1-.3-.2-.7-.4-1.1l-4.9-3c-.3-.2-.5-.6-.5-.9v-2.4c-.2-.1-.4-.3-.5-.4-.2-.1-.4 0-.4.3v2z"/>
      </g>
      <g id="XMLID_35_">
        <path class="st219" d="M950.8 3489.2c-.1.1-.2.2-.1.5l1.2 6.2c.1.4.3.7.6.8l.6.2h.4c.1-.1.1-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.4z"/>
        <path class="st227" d="M950.8 3489.2h.2l.6.2c.3.1.5.4.6.8l1.2 6.2c0 .2 0 .4-.1.5l.2-.1 2.5-1.5.5-.3 3.7-2.2c.1-.1.2-.2.1-.5l-.1-.3c-.2-.1-.5-.4-.5-.8l-1.1-5.9h-.1l-.6-.2h-.2l-6.9 4.1z"/>
        <path class="st219" d="M952.8 3500.9v.9c0 .4.3.9.6 1.1l7.9 4.8c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.2-.2.3-.2.5z"/>
        <path class="st226" d="M953 3500.5c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l6.8-4.1c.1-.1.2-.2.2-.4v-.5l-7.5-4.5c-.3-.2-.6-.7-.6-1.1v-.5l-.4-.2c-.1-.1-.2-.1-.3-.1h-.1l-2.5 1.5-.4.3-2.5 1.5-.4.3-1.1.5z"/>
        <path class="st92" d="M953 3496.8l.2 1.4c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.2.1h-.1c0 .1 0 .1-.2 0zm3-1.6l.2 1.2c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.5.3z"/>
        <path class="st222" d="M958.7 3484.4c-.1.1-.2.2-.1.5l.1.3c.2.1.5.4.5.8l1.1 5.9h.1l.6.2h.4c.1-.1.1-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.4z"/>
        <path class="st226" d="M958.6 3485.2l1.1 5.9c.1.3.3.7.5.8l-1.1-5.9c0-.4-.2-.7-.5-.8zm.1-.8h.2l.6.2c.3.1.5.4.6.8l1.2 6.2c0 .2 0 .4-.1.5l.2-.1 2.5-1.5.5-.3 3.7-2.2c.1-.1.2-.2.1-.5l-1.2-6.2c-.1-.4-.3-.7-.6-.8l-.6-.2h-.2l-6.9 4.1zm2 12.2v.5c0 .4.3.9.6 1.1l7.5 4.5v-.5c0-.4-.3-.9-.6-1.1l-7.5-4.5z"/>
        <path class="st222" d="M960.7 3496.2v.5l7.5 4.5c.3.2.6.7.6 1.1v.5l.4.2c.2.1.3.1.5 0 .1-.1.1-.2.1-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.2-.1-.3-.1-.4-.1-.1.1-.2.3-.2.5z"/>
        <path class="st226" d="M960.9 3495.7c.1 0 .3 0 .4.1l7.9 4.8c.3.2.6.7.6 1.1v.9c0 .2-.1.3-.1.4l6.8-4.1c.1-.1.2-.2.2-.4v-.9c0-.4-.3-.9-.6-1.1l-7.9-4.8c-.1-.1-.2-.1-.3-.1h-.1l-2.5 1.5-.4.3-2.5 1.5-.4.3-1.1.5z"/>
        <path class="st92" d="M960.9 3492.1l.2 1.4c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.2.1h-.3zm3-1.7l.2 1.2c.1.6.4 1.2.8 1.7l.4-.3c-.3-.3-.6-.8-.6-1.2l-.3-1.7-.5.3z"/>
      </g>
      <g id="XMLID_34_">
        <path class="st223" d="M950.8 3497.7v3.1c0 1 .7 2.2 1.5 2.7l5.9 3.6c.4.2.7.3 1 .1 0 0 .1 0 .1-.1l.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1-.2h-.1c-.2.3-.4.6-.4 1.1zm1 3.7v-3.1c0-.3.2-.4.4-.3.2.1.4.3.5.4 2.4 1.8 4.5 4.2 5.4 6.3.2.4.3.7.4 1.1v.2c-.1.1-.2.1-.3 0l-5.9-3.6c-.2-.2-.5-.6-.5-1z"/>
        <path class="st218" d="M952.2 3496.2l-.9.5c.3-.1.6-.1 1 .2 3.5 2.4 6.4 6 7.2 9 .1.5.1.9-.1 1.2l-.1.1.9-.5.1-.1.1-.1c.2-.2.3-.7.1-1.2-.8-3-3.6-6.6-7.2-9-.4-.3-.8-.3-1.1-.1z"/>
        <path class="st214" d="M951.8 3500.2v1.2c0 .3.2.7.5.9l5.9 3.6c.2.1.3.1.3 0v-.2c-.1-.3-.2-.7-.4-1.1l-4.9-3c-.3-.2-.5-.6-.5-.9v-2.4c-.2-.1-.4-.3-.5-.4-.2-.1-.4 0-.4.3v2z"/>
      </g>
      <path class="st214" d="M974.3 3504c.2-.1.4-.1.7.1l.7.4-1.5.9-2.4 1.5-.7-.4c-.3-.2-.5-.2-.7-.1l3.9-2.4z"/>
      <path class="st92" d="M970.1 3507c0 .2.1.5.2.7l1.5-.9-.7-.4c-.3-.2-.5-.2-.7-.1-.2.1-.3.4-.3.7zm1.8-.9s.2.2.6-.1c.2-.1 0-.3 0-.3l-7.1-11.5-.6.4 7.1 11.5z"/>
      <path class="st92" d="M961.9 3496.9c.1 0 .3-.1.5-.2h.1c.3-.1.8-.5 1.1-.6h.1c.4-.2 1.2-.7 1.6-1 .4-.3 1.2-.8 1.7-1.1l.1-.1c.3-.2.9-.6 1.1-.9l.1-.1c.3-.2.6-.5.4-.8-.1-.1-.2-.2-.3-.2-.1 0-.3.1-.5.2h-.1c-.3.1-.8.5-1.1.6h-.1c-.4.2-1.2.8-1.6 1-.4.3-1.3.8-1.7 1.1l-.1.1c-.3.2-.9.6-1.1.9l-.1.1c-.3.3-.6.5-.4.8 0 .1.1.2.3.2z"/>
      <g id="XMLID_33_">
        <path class="st228" d="M972.9 3507.5l.4 1.3 14.5-8.8-.7-.6-.1-.5z"/>
        <path class="st216" d="M973.3 3508.8l.1.5 14.8-9 .2-.6z"/>
        <path class="st228" d="M987 3499l.1.4.7.6.3-.1z"/>
      </g>
      <path class="st216" d="M989.2 3499.7c0-.1-.3-5.2-.8-8.8-.6-4.9-3.8-9.4-6.5-11.3-4.9-3.6-41.7-24-41.9-24l-1.3-.8c-.9-.4-2.7-1.1-4.9.2-1.4.9-2.2 2.6-2.6 4.9l.9.1c.3-1.9 1-3.3 2-4 1.5-.9 3.8-.1 4.1.1 1.1.6 38.5 22.1 42.6 24.7 5.8 3.6 7 19.7 7 19.7l1.4-.8z"/>
      <path class="st215" d="M988 3499.9c0-.4-.3-5.4-.8-9.1-.6-4.8-4-9.6-6.8-11.2-4.2-2.4-42.5-24-42.7-24.1-.1-.1-2.4-1.3-4.3-.1-1.3.8-2.1 3-2.2 5.4l1.2.5c.1-1.9.8-4.2 1.7-4.7 1.2-.7 2.9.1 3.1.2.7.4 36.7 21.5 41.1 23.3 9 3.6 8.7 18.9 8.7 19.1l1 .7z"/>
      <path class="st216" d="M973.6 3509.1c0-.1.3-2.4-.2-6-.6-4.9-3.5-12.3-6.9-14.2-5.3-2.9-41.9-24-42.1-24l-1.3-.8c-.9-.4-2-1.4-5.6.6-1.5.8-3.4 20.5-3.7 22.8l.9-.5c.9-5.8 2.4-19.5 3.6-20.9 1.2-1.4 3-.2 3.3-.1 1.1.6 39.7 21.6 43.9 24.2 5.8 3.6 6.8 19.7 6.8 19.7l1.3-.8z"/>
      <path class="st216" d="M930.4 3471c-1.8-1.1-3.9-1.8-5.6-3.1-1.6-1.3-3.6-2.5-5.6-2.7-.4 0-.6.1-.8.3-.7-.4-.8-.8-.8-.8l16.3-9.8 2.9-.7c.7.4 40.3 22.9 44.7 25.6 0 0 2.8 2.3 3.3 3.5l-16.9 8.6.1.5c-.7-.7-1.6-2.4-2.5-2.9-.8-.4-20.7-10.5-34.7-17.7 0-.2-.1-.6-.4-.8z"/>
      <path class="st229" d="M984.2 3483.4s-9.3 3.2-15.3 8c0 0 .6.6 1 1.4 0 0 6.6-5.1 15.2-7.9.1 0-.4-.9-.9-1.5z"/>
      <linearGradient id="SVGID_11_" gradientUnits="userSpaceOnUse" x1="4042.867" y1="3484.89" x2="4042.867" y2="3508.566" gradientTransform="matrix(-.477 0 0 1 2906.666 0)">
        <stop offset="0" stop-color="#FFF" stop-opacity="0"/>
        <stop offset="1" stop-opacity=".4"/>
      </linearGradient>
      <path class="st242" d="M988 3499.9s-.5-12.4-2.9-15c0 0-9.1 2.8-15.2 7.9 0 0 3.9 5.6 3.7 15.7l14.4-8.6z"/>
      <path class="st215" d="M972.4 3509.9c-.1.7.3-3.1-.2-6.9-.6-4.8-3.4-11.9-7.1-14-4.2-2.4-42.7-24-42.9-24.1-.1-.1-2.4-1.3-4.3-.1-1.3.8-1.9 2.7-2.1 5.7l.9.3c.6-3.8 1-4.3 1.8-4.9 1.2-.7 2.9.2 3.1.3.7.4 38.6 21.9 42.9 24.1 7 3.8 7 18.7 7 18.8l.9.8z"/>
      <path class="st215" d="M916.7 3470.2h-1l-2.6 16.7.8.7z"/>
    </g>
    <g id="building">
      <path class="st243" d="M1560.4 1745.7l199-113.2 142.8 82.2-199.2 112.6-142.6-81.6z"/>
      <path class="st244" d="M1560.4 1745.7l.2-285.1 74.3 42.7 68.5 39.4-.5 284.5-74-42.1v-.5l-68.5-38.9z"/>
      <path class="st245" d="M1560.6 1460.6l142.8 82.2 73.8-42.8-142.3-82.2z"/>
      <path class="st246" d="M1777.2 1500l-73.8 42.7-.5 284.5 74-42.1.3-285.1z"/>
      <path class="st11" d="M1560.4 1745.7l.2-285.1 142.8 82.2-.5 284.5-142.5-81.6z"/>
      <path class="st247" d="M1560.6 1460.6l142.8 82.2 73.8-42.8-142.3-82.2z"/>
      <path class="st248" d="M1740.4 1473.4l-48.7 28.2-.3 16.1 48.9-27.8.1-16.5z"/>
      <path class="st11" d="M1597.3 1463.8l.1-16.5 94.3 54.3-.3 16.1-94.1-53.9z"/>
      <path class="st247" d="M1597.4 1447.3l94.3 54.3 48.7-28.2-93.9-54.3z"/>
      <path class="st20" d="M1568 1471.6v6.3l5.5 3.2.1-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm0 8.5v6.4l5.5 3.1v-6.3zm0 8.6v6.3l5.5 3.1v-6.3zm-.2 42.6v6.3l5.5 3.2.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm-.1 59.7v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 25.6v6.3l5.5 3.2.1-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm0 8.6v6.3l5.5 3.2v-6.4zm0 8.5v6.3l5.5 3.2v-6.3zm0 8.5l-.1 6.3 5.5 3.2.1-6.3zm-.1 25.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.1 34.2v6.3l5.5 3.1v-6.3zm.1-8.6l-.1 6.3 5.6 3.2v-6.3zm-.1 25.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm-.1 51.1l-.1 6.4 5.6 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm.1-8.6l-.1 6.3 5.6 3.2v-6.3zm-.2 59.7v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1.1-6.3zm9.5-233.7v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm-.1 51.2l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm-.2 42.6v6.3l5.5 3.2v-6.3zm0 25.6l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.1 25.6v6.3l5.5 3.2v-6.3zm0 8.5v6.4l5.5 3.1v-6.3zm-.1 34.2v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm-.2 68.2v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.3 93.8v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.3l5.5 3.2.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.3zm-.2 59.7v6.3l5.5 3.2v-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm0 8.6l-.1 6.3 5.5 3.1.1-6.3zm9.5-259.3v6.3l5.5 3.2v-6.4zm-.1 25.5v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm0 25.6v6.3l5.5 3.2v-6.4zm-.1 17v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm0 17.1v6.3l5.5 3.1v-6.3zm-.1 42.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.3zm-.1 42.6l-.1 6.3 5.5 3.2.1-6.3zm-.1 17.1v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0 25.6l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 17v6.4l5.5 3.1v-6.3zm0 8.6v6.3l5.5 3.2v-6.3zm0 17l-.1 6.4 5.6 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 34.1v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm-.1 34.1v6.3l5.5 3.2.1-6.4zm.1-8.6l-.1 6.4 5.6 3.1v-6.3zm-.1 25.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 34.1v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.4zm.1-8.6l-.1 6.4 5.6 3.1v-6.3zm18.2-237.1v6.3l5.5 3.1v-6.3zm0 8.5l-.1 6.3 5.6 3.2v-6.4zm-.1 8.5v6.3l5.5 3.2.1-6.3zm-.1 34.1v6.3l5.5 3.2.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.3l5.5 3.2v-6.3zm-.1 42.7v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.1 25.6v6.3l5.5 3.2.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.3zm-.2 76.7l-.1 6.4 5.6 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm.1-8.6l-.1 6.3 5.5 3.2.1-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.2 76.8v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm-.1 34.1v6.3l5.5 3.2.1-6.4zm.1-8.6l-.1 6.4 5.6 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 25.6v6.3l5.5 3.2v-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm0 8.6l-.1 6.3 5.6 3.1v-6.3zm-.1 8.5v6.3l5.5 3.2v-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm-.1 17.1v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.1v-6.3zm9.4-233.8v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm-.2 51.1v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm-.1 34.1v6.3l5.5 3.2v-6.3zm-.1 34.1v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm-.2 42.6v6.4l5.5 3.1.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm-.1 17.1v6.3l5.5 3.2v-6.4zm0 8.5v6.3l5.5 3.2v-6.3zm-.1 17v6.4l5.5 3.1.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm-.1 17.1v6.3l5.5 3.2v-6.3zm0 17v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 34.1v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1.1-6.3zm0 25.5v6.4l5.5 3.1v-6.3zm-.1 8.6v6.3l5.5 3.2.1-6.4zm0 8.5v6.3l5.5 3.2v-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm0 8.5v6.4l5.5 3.1v-6.3zm0 8.6l-.1 6.3 5.5 3.2.1-6.4zm-.1 17v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm9.4-225.2v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.1 42.7v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.1 25.6v6.3l5.5 3.2.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.3zm-.2 51.2v6.3l5.5 3.2v-6.4zm.1-8.6l-.1 6.3 5.5 3.2.1-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm-.1 51.1v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.2 59.7v6.3l5.5 3.2v-6.4zm.1-8.6l-.1 6.4 5.6 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm.1-8.6l-.1 6.4 5.5 3.1.1-6.3zm-.2 59.7v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0 17l-.1 6.4 5.6 3.1v-6.3zm-.1 25.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0 25.6l-.1 6.3 5.6 3.1v-6.3zm-.1 17v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm0 17v6.4l5.5 3.1v-6.3zm0 8.6l-.1 6.3 5.6 3.2v-6.4zm18.2-245.8v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm0 25.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm-.1 34.1v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2.1-6.3zm-.1 51.2v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm.1-8.6l-.1 6.4 5.5 3.1.1-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 34.1v6.3l5.5 3.2v-6.3zm-.1 34.1v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm.1-8.6l-.1 6.4 5.5 3.1.1-6.3zm-.2 51.2v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm.1-8.5l-.1 6.3 5.5 3.1.1-6.3zm-.1 25.5v6.3l5.5 3.2v-6.3zm-.1 17.1v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.4zm-.1 17v6.3l5.5 3.2v-6.3zm0 17.1l-.1 6.3 5.6 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.1 25.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm0 25.6l-.1 6.3 5.6 3.2v-6.4zm0-8.5v6.3l5.5 3.1v-6.3zm-.1 34.1v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm9.5-233.7v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm-.1 25.5v6.4l5.5 3.1.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm-.1 17.1v6.3l5.5 3.2v-6.4zm0 17l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 42.6l-.1 6.4 5.6 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1.1-6.3zm-.1 42.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1.1-6.3zm-.2 68.2v6.3l5.5 3.2.1-6.3zm.1-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.4zm.1-8.6l-.1 6.4 5.6 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.2 59.7v6.3l5.5 3.2v-6.3zm0 17.1v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm0 17.1l-.1 6.3 5.5 3.2.1-6.3zm-.1 8.5v6.3l5.5 3.2v-6.3zm0 8.5v6.4l5.5 3.1v-6.3zm0 8.6v6.3l5.5 3.2v-6.4zm0 8.5l-.1 6.3 5.6 3.2v-6.3zm-.1 17v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0 25.6l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm9.4-242.3v6.4l5.5 3.1.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.3zm-.1 17.1v6.3l5.5 3.2v-6.4zm0 17v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.2 51.1v6.4l5.5 3.1.1-6.3zm.1-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1.1-6.3zm-.1 51.2v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm-.1 42.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm.1-8.5l-.1 6.3 5.5 3.1.1-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm-.2 68.2v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.2 76.8l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.4zm-.2 42.6v6.3l5.5 3.2.1-6.3zm0 8.5v6.4l5.5 3.1v-6.3zm0 17.1l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm-.1 25.5v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm-60.6-291.1l-.7 270.7 5.5 3.1.7-270.6zm35.1 20.2l-.8 270.6 5.5 3.2.8-270.6zm35 20.1l-.7 270.7 5.5 3.2.7-270.7zm8.8 5.1v6.3l5.5 3.2v-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm-.1 17.1v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1.1-6.3zm-.1 42.7v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1.1-6.3zm.1-8.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 51.2l-.1 6.3 5.5 3.2.1-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 51.2l-.1 6.3 5.6 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 59.7l-.1 6.3 5.6 3.2v-6.4zm0-8.5v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 34.1v6.3l5.5 3.2.1-6.3zm0 8.5v6.3l5.5 3.2v-6.3zm-.1 25.6v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm-.1 34.1v6.3l5.5 3.1v-6.3zm0-8.6v6.4l5.5 3.1v-6.3zm0 17.1l-.1 6.3 5.6 3.2v-6.3zm-.1 8.5v6.3l5.5 3.2.1-6.3zm0 17.1v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0 17.1l-.1 6.3 5.6 3.2v-6.3zm-.1 8.5v6.3l5.5 3.2.1-6.3zm9.5-233.7v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm.1-8.6l-.1 6.4 5.6 3.1v-6.3zm-.2 42.7v6.3l5.5 3.2.1-6.4zm.1-8.6l-.1 6.4 5.6 3.1v-6.3zm-.1 34.2v6.3l5.5 3.1v-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.2 59.7v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.1v-6.3zm0-8.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm-.1 59.7v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 25.6v6.3l5.5 3.2.1-6.3zm0 25.6v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0 25.6l-.1 6.3 5.5 3.2.1-6.3zm-.1 8.5v6.3l5.5 3.2v-6.3zm0 17.1v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm-.1 42.6v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm0 34.1l-.1 6.3 5.5 3.2.1-6.3zm-.1 17.1v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm9.5-233.7v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0 25.6l-.1 6.3 5.5 3.2.1-6.4zm-.2 42.6v6.3l5.5 3.2v-6.3zm.1-8.5l-.1 6.3 5.5 3.2.1-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm-.1 42.6v6.3l5.5 3.2v-6.3zm-.1 25.6v6.3l5.5 3.2v-6.3zm.1-8.5l-.1 6.3 5.5 3.2.1-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm-.1 25.6v6.3l5.5 3.2v-6.3zm-.1 34.1v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.4zm0-8.5v6.3l5.5 3.2v-6.4zm-.2 68.2v6.3l5.5 3.2v-6.4zm0-8.6v6.4l5.5 3.1v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm-.2 51.1v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm-.2 42.6v6.3l5.5 3.2.1-6.3zm.1-8.5l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm0-8.5v6.3l5.5 3.1v-6.3zm-.1 34.1v6.3l5.5 3.1v-6.3zm0 17l-.1 6.3 5.6 3.2v-6.3zm0-8.5v6.3l5.5 3.2v-6.3zm80.3-286.8v6.3l-5.5 3.2-.1-6.3zm0 8.5v6.3l-5.5 3.2v-6.3zm0 8.6v6.3l-5.5 3.1v-6.3zm.1 34.1v6.3l-5.5 3.1v-6.3zm0-8.6v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.4zm.2 42.6v6.3l-5.5 3.2-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.3zm.1 25.6v6.3l-5.5 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm.2 76.8v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.1v-6.3zm-.1-8.6l.1 6.3-5.6 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm-.1-8.5l.1 6.3-5.5 3.2-.1-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.2 76.7l.1 6.3-5.5 3.2-.1-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.1 34.1v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm0 25.5l.1 6.4-5.6 3.1v-6.3zm.1 8.6v6.3l-5.5 3.2v-6.4zm0 8.5v6.3l-5.5 3.2v-6.3zm0 8.5v6.3l-5.5 3.2v-6.3zm0 8.5l.1 6.4-5.6 3.1v-6.3zm.1 8.6v6.3l-5.5 3.2-.1-6.4zm0 17v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm-9.5-233.7l.1 6.3-5.6 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm.1 51.2l.1 6.3-5.6 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.6v6.4l-5.5 3.1v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.1 34.1v6.3l-5.5 3.2v-6.3zm.1 34.1v6.4l-5.5 3.1-.1-6.3zm-.1-8.5l.1 6.3-5.6 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.1v-6.3zm.1 42.6v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm0 17l.1 6.3-5.6 3.2v-6.3zm.1 8.5v6.4l-5.5 3.1v-6.3zm0 17.1v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm0 17l.1 6.3-5.6 3.2v-6.3zm.1 17.1v6.3l-5.5 3.2v-6.3zm0-8.6v6.4l-5.5 3.1-.1-6.3zm.1 34.2v6.3l-5.5 3.1-.1-6.3zm-.1-8.6l.1 6.3-5.6 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.1 25.6v6.3l-5.5 3.2v-6.3zm0 8.5v6.3l-5.5 3.2v-6.3zm0 8.5l.1 6.4-5.6 3.1v-6.3zm.1 8.6v6.3l-5.5 3.2-.1-6.4zm0 8.5v6.3l-5.5 3.2v-6.3zm0 8.5v6.3l-5.5 3.2v-6.3zm0 17.1l.1 6.3-5.5 3.2-.1-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm-9.4-225.1v6.3l-5.5 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm0-8.5v6.3l-5.5 3.2-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.3zm.2 42.6v6.3l-5.5 3.2-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.3zm.1 25.6v6.3l-5.5 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm.1 51.2v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.1v-6.3zm0-8.6v6.3l-5.5 3.2-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.3zm.2 51.2v6.3l-5.5 3.1v-6.3zm0-8.6v6.3l-5.5 3.2-.1-6.3zm.1 59.7v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm-.1-8.6l.1 6.4-5.5 3.1-.1-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.2 59.7v6.3l-5.5 3.2v-6.4zm-.1-8.6l.1 6.4-5.5 3.1-.1-6.3zm.1 17.1v6.3l-5.5 3.2v-6.3zm.1 25.6v6.3l-5.5 3.2-.1-6.3zm-.1-8.5l.1 6.3-5.6 3.1v-6.3zm0-8.6v6.3l-5.5 3.2v-6.3zm.1 25.6v6.3l-5.5 3.2v-6.3zm0 17.1l.1 6.3-5.6 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm.1 17.1v6.3l-5.5 3.2-.1-6.3zm0 8.5v6.3l-5.5 3.2v-6.3zm-18.3-245.7l.1 6.3-5.6 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm.1 25.5v6.4l-5.5 3.1v-6.3zm0-8.5v6.3l-5.5 3.2-.1-6.3zm.1 34.1v6.3l-5.5 3.2-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm.2 51.1v6.4l-5.5 3.1-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.1v-6.3zm.1 34.1v6.3l-5.5 3.2v-6.4zm.1 34.1v6.3l-5.5 3.2v-6.4zm-.1-8.6l.1 6.4-5.5 3.1-.1-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.1 51.1l.1 6.4-5.6 3.1v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.1 25.6v6.3l-5.5 3.2v-6.3zm0 17v6.4l-5.5 3.1v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0 17.1l.1 6.3-5.6 3.1v-6.3zm.1 17v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0 25.6l.1 6.3-5.6 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm.1 25.6v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2-.1-6.3zm.1 34.1v6.3l-5.5 3.2-.1-6.3zm-.1-8.5l.1 6.3-5.6 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm-9.4-233.7v6.4l-5.5 3.1v-6.3zm-.1-8.5l.1 6.3-5.6 3.2v-6.3zm.1 25.6v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm0 17l.1 6.3-5.6 3.2v-6.3zm.1 17.1v6.3l-5.5 3.2v-6.3zm0-8.6v6.4l-5.5 3.1v-6.3zm.1 42.7v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.1-.1-6.3zm-.1-8.6l.1 6.3-5.6 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.1 42.6l.1 6.4-5.6 3.1v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.2 68.2v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2-.1-6.4zm-.1-8.6l.1 6.4-5.6 3.1v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2-.1-6.4zm.1 59.7v6.3l-5.5 3.1v-6.3zm.1 17v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2-.1-6.3zm0 17v6.3l-5.5 3.2v-6.3zm0 8.6v6.3l-5.5 3.1v-6.3zm.1 8.5v6.3l-5.5 3.2-.1-6.3zm0 8.5v6.3l-5.5 3.2v-6.3zm0 8.5v6.4l-5.5 3.1v-6.3zm0 17.1l.1 6.3-5.5 3.2-.1-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm.1 25.5v6.4l-5.5 3.1v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm-9.5-242.2v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.1v-6.3zm0 17l.1 6.3-5.6 3.2v-6.3zm.1 17.1v6.3l-5.5 3.2v-6.4zm0-8.6v6.4l-5.5 3.1-.1-6.3zm.1 51.2v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm0-8.6v6.4l-5.5 3.1-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.2 51.1v6.4l-5.5 3.1-.1-6.3zm-.1-8.5v6.3l-5.5 3.2v-6.3zm.1 42.7l.1 6.3-5.5 3.1-.1-6.3zm0-8.6v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm.2 68.2v6.3l-5.5 3.2v-6.3zm-.1-8.5l.1 6.3-5.6 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.2 76.7v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm-.1-8.5l.1 6.3-5.6 3.2v-6.4zm0-8.6v6.4l-5.5 3.1v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm.1 42.7v6.3l-5.5 3.1v-6.3zm0 8.5l.1 6.3-5.6 3.2v-6.3zm.1 17v6.3l-5.5 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.3zm0 25.6l.1 6.3-5.6 3.2v-6.3zm0-8.5v6.3l-5.5 3.2v-6.4zm25.6-271l.7 270.7-5.5 3.1-.7-270.6z"/>
    </g>
    <path class="st6" d="M504.7 2170.9c1.7 1 1.7 2.5 0 3.5s-4.4 1-6 0c-1.7-1-1.7-2.5 0-3.5 1.6-1 4.3-1 6 0z"/>
    <path class="st249" d="M565 2189c2.2 1.3 2.2 3.4 0 4.7-2.2 1.3-5.8 1.3-8.1 0-2.2-1.3-2.2-3.4 0-4.7 2.3-1.3 5.9-1.3 8.1 0z"/>
    <path class="st6" d="M587.5 2229.8c1.5.9 1.5 2.3 0 3.2-1.5.9-4 .9-5.5 0s-1.5-2.3 0-3.2c1.5-.9 4-.9 5.5 0zm7.2-31.5c1.1.6 1.1 1.6 0 2.3-1.1.6-2.8.6-3.9 0s-1.1-1.6 0-2.3c1.1-.6 2.9-.6 3.9 0z"/>
    <path class="st249" d="M499.3 2136.1c3.1 1.8 3.1 4.6 0 6.4-3 1.8-8 1.8-11.1 0-3.1-1.8-3.1-4.6 0-6.4 3.1-1.8 8.1-1.8 11.1 0z"/>
    <path class="st6" d="M454.2 2133.9c4.5 2.6 4.5 6.8.1 9.5-4.5 2.6-11.8 2.6-16.3 0s-4.5-6.8-.1-9.5c4.5-2.6 11.8-2.6 16.3 0zM697 3486.5c1.7 1 1.7 2.5 0 3.5s-4.4 1-6 0c-1.7-1-1.7-2.5 0-3.5s4.4-1 6 0z"/>
    <path class="st249" d="M757.4 3504.7c2.2 1.3 2.2 3.4 0 4.7-2.2 1.3-5.8 1.3-8.1 0-2.2-1.3-2.2-3.4 0-4.7 2.2-1.3 5.9-1.3 8.1 0z"/>
    <path class="st6" d="M779.9 3545.4c1.5.9 1.5 2.3 0 3.2-1.5.9-4 .9-5.5 0s-1.5-2.3 0-3.2c1.5-.8 3.9-.8 5.5 0zm7.2-31.5c1.1.6 1.1 1.6 0 2.3-1.1.6-2.8.6-3.9 0s-1.1-1.6 0-2.3c1.1-.6 2.8-.6 3.9 0z"/>
    <path class="st249" d="M691.7 3451.7c3.1 1.8 3.1 4.6 0 6.4-3 1.8-8 1.8-11.1 0-3.1-1.8-3.1-4.6 0-6.4 3.1-1.7 8-1.7 11.1 0z"/>
    <path class="st6" d="M646.6 3449.5c4.5 2.6 4.5 6.8.1 9.5-4.5 2.6-11.8 2.6-16.3 0s-4.5-6.8-.1-9.4c4.5-2.7 11.8-2.7 16.3-.1zm1205.8-1566c1.7 1 1.7 2.5 0 3.5s-4.4 1-6 0c-1.7-1-1.7-2.5 0-3.5 1.6-.9 4.3-.9 6 0z"/>
    <path class="st249" d="M1912.7 1901.7c2.2 1.3 2.2 3.4 0 4.7-2.2 1.3-5.8 1.3-8.1 0-2.2-1.3-2.2-3.4 0-4.7 2.3-1.3 5.9-1.3 8.1 0z"/>
    <path class="st6" d="M1935.2 1942.5c1.5.9 1.5 2.3 0 3.2-1.5.9-4 .9-5.5 0s-1.5-2.3 0-3.2c1.5-.9 4-.9 5.5 0zm7.2-31.6c1.1.6 1.1 1.6 0 2.3-1.1.6-2.8.6-3.9 0s-1.1-1.6 0-2.3c1.1-.6 2.8-.6 3.9 0z"/>
    <path class="st249" d="M1847 1848.7c3.1 1.8 3.1 4.6 0 6.4-3 1.8-8 1.8-11.1 0-3.1-1.8-3.1-4.6 0-6.4 3.1-1.7 8.1-1.7 11.1 0z"/>
    <path class="st6" d="M1801.9 1846.6c4.5 2.6 4.5 6.8.1 9.5-4.5 2.6-11.8 2.6-16.3 0s-4.5-6.8-.1-9.5c4.5-2.7 11.8-2.7 16.3 0z"/>
    <g class="st250">
      <path class="st6" d="M1493 262.1c1.5.9 1.5 2.3-.1 3.1-1.6.8-4.2.6-5.7-.3-1.5-.9-1.5-2.3.1-3.1 1.6-.8 4.2-.6 5.7.3z"/>
      <path class="st249" d="M1440.5 266.9c2.1 1.2 2 3.1-.2 4.1-2.2 1-5.6.9-7.7-.4-2.1-1.2-2-3.1.2-4.1 2.2-1 5.6-.8 7.7.4z"/>
      <path class="st6" d="M1505.6 239.2c1.4.9 1.4 2.1-.1 2.8-1.5.7-3.8.6-5.3-.3-1.4-.9-1.4-2.1.1-2.8 1.5-.7 3.8-.6 5.3.3zm-41.6 4.9c1 .6 1 1.5-.1 2-1 .5-2.7.4-3.7-.2-1-.6-1-1.5.1-2s2.7-.4 3.7.2z"/>
      <path class="st249" d="M1425.1 300.9c2.8 1.7 2.7 4.3-.2 5.7-3 1.4-7.7 1.2-10.5-.5s-2.7-4.3.2-5.7c3-1.5 7.7-1.2 10.5.5z"/>
      <path class="st6" d="M1371.7 300.7c4.2 2.5 4 6.3-.4 8.4-4.4 2.1-11.3 1.7-15.5-.8-4.2-2.5-4-6.3.4-8.4 4.3-2.1 11.3-1.7 15.5.8z"/>
    </g>
    <g class="st250">
      <path class="st6" d="M63 1083.6c-1.7-1-1.6-2.5.1-3.4 1.8-.8 4.6-.7 6.3.3 1.7 1 1.6 2.5-.1 3.4-1.8.8-4.6.7-6.3-.3z"/>
      <path class="st249" d="M120.8 1078.3c-2.3-1.4-2.2-3.4.2-4.5 2.4-1.1 6.2-.9 8.4.4 2.3 1.4 2.2 3.4-.2 4.5-2.4 1.1-6.2.9-8.4-.4z"/>
      <path class="st6" d="M49.2 1108.7c-1.6-.9-1.5-2.3.1-3.1 1.6-.8 4.2-.6 5.8.3 1.6.9 1.5 2.3-.1 3.1-1.6.7-4.2.6-5.8-.3zm45.7-5.4c-1.1-.7-1.1-1.6.1-2.2 1.2-.5 3-.5 4.1.2 1.1.7 1.1 1.6-.1 2.2-1.2.6-3 .5-4.1-.2z"/>
      <path class="st249" d="M137.6 1041.1c-3.1-1.9-3-4.7.3-6.2 3.3-1.6 8.5-1.3 11.6.6 3.1 1.9 3 4.7-.3 6.2-3.2 1.5-8.4 1.3-11.6-.6z"/>
      <path class="st6" d="M196.4 1041.3c-4.6-2.8-4.4-6.9.4-9.2 4.8-2.3 12.5-1.9 17.1.9 4.6 2.8 4.4 6.9-.4 9.2-4.8 2.2-12.5 1.9-17.1-.9z"/>
    </g>
    <g class="st250">
      <path class="st6" d="M1329.9 2849c-1.3-.7-1.3-1.8.1-2.5 1.4-.6 3.5-.5 4.8.2 1.3.7 1.3 1.8-.1 2.5-1.4.6-3.5.5-4.8-.2z"/>
      <path class="st249" d="M1374.1 2845.2c-1.7-1-1.7-2.5.1-3.3 1.8-.8 4.7-.7 6.5.3 1.7 1 1.7 2.5-.1 3.3-1.9.9-4.8.7-6.5-.3z"/>
      <path class="st6" d="M1319.4 2867.2c-1.2-.7-1.2-1.7.1-2.3 1.2-.6 3.2-.5 4.4.2 1.2.7 1.2 1.7-.1 2.3-1.2.6-3.2.5-4.4-.2zm34.9-3.8c-.8-.5-.8-1.2.1-1.6.9-.4 2.3-.3 3.1.2.8.5.8 1.2-.1 1.6-.8.3-2.2.3-3.1-.2z"/>
      <path class="st249" d="M1386.9 2818.3c-2.4-1.4-2.3-3.4.2-4.5s6.5-.9 8.9.4c2.4 1.4 2.3 3.4-.2 4.5-2.5 1.2-6.5 1-8.9-.4z"/>
      <path class="st6" d="M1431.9 2818.5c-3.5-2-3.4-5 .3-6.7 3.7-1.7 9.5-1.4 13.1.7 3.5 2 3.4 5-.3 6.7-3.7 1.6-9.5 1.4-13.1-.7z"/>
    </g>
    <g id="evening-hours">
      <text transform="matrix(.992 0 0 1 1037.664 1907.78)" class="st89 st90 st91">
        Evening Hours
      </text>
      <text transform="matrix(.992 0 0 1 1037.664 1947.086)">
        <tspan x="0" y="0" class="st92 st93 st165">In the evening, the service shifts to accommodate requests on demand – </tspan><tspan x="0" y="24.5" class="st92 st93 st165">users can use the app to request pick-ups and be transported anywhere</tspan><tspan x="0" y="49" class="st92 st93 st165">within a predetermined distance from the university campus. We hope</tspan><tspan x="0" y="73.4" class="st92 st93 st165">to improve overall safety and peace of mind by eliminating the need to</tspan><tspan x="0" y="97.9" class="st92 st93 st165">drink and drive and reduce campus crime.</tspan>
      </text>
      <g id="evening-icon-1">
        <path class="st251" d="M1191.4 2174.4h-58.1l1.1-4.7.8-3.4.5-2c.3-1.1.8-2 1.7-2.7l.2-.2 2.4-1.9 1.6-1.3 4.6-3.8 1-.9 1.6-1.4h27.1l1.6 1.4 1 .9 4.6 3.8 1.6 1.3 2.4 1.9c.1.1.2.1.2.2.8.7 1.4 1.6 1.7 2.7l.5 2 .8 3.4 1.1 4.7z"/>
        <path class="st252" d="M1191.4 2174.4h-58.1l1.1-4.7h55.9zm-1.9-8.1h-54.3l.5-2c.3-1.1.8-2 1.7-2.7h50c.8.7 1.4 1.6 1.7 2.7l.4 2zm-6.4-8.1h-41.5l4.6-3.9 1-.8h30.3l1 .8z"/>
        <path class="st126" d="M1148.8 2134.1s0 .1 0 0c-.5.4-2.3 1.6-3.2-3 0-.1 0-.2-.1-.2-1-5-1.1-8.1.1-9.4.2-.3.5-.5.9-.6.7-.2 1.1-.1 1.3.2.3.2.4.5.4.5l.3 5.3.2 4.2.1 3z"/>
        <path class="st253" d="M1153.4 2145.7l-1.8 2-2.8 3.1c-.2.2-.3.5-.3.8 0 .3.2.5.4.7 1.7 1.4 5.9 4.6 10 5.4 0 0-8.3.5-12.9-2.2-.8-.5-1.8-.6-2.5 0l-4.5 3.4-.8 2 .7-.6c.2-.2.5-.2.8-.2.3.1.5.3.7.5 1.2 2.3 4.9 7.5 12.8 7.5 10.2 0 21.2-10.9 24.9-11.8 2.5-.6 5.6 2.5 5.6 2.5l-.2-.5c-.3-.7-.8-1.4-1.5-1.9l-2.9-2.1c-.9-.6-2-.9-3.1-.7v-.3c0-1-.3-1.9-1-2.7l-2.4-3-2-1.7-17.2-.2z"/>
        <path class="st126" d="M1153.3 2141.6v1.6c0 2.9.9 9.4 9 9.3 7.3-.1 8.6-6.4 8.6-9.3v-2l-17.6.4z"/>
        <path class="st127" d="M1153.4 2145.7c2.4 2.7 5.2 4.1 8.5 4.1 3.5 0 6.5-1.7 9-4.6l.1-3-17.7.4.1 3.1z"/>
        <path class="st128" d="M1161.9 2147.7c8.1 0 14.2-8.5 14.2-22.6 0-17.6-5.1-21.7-14.2-21.7s-14.2 4.1-14.2 21.7c0 14.1 6.2 22.6 14.2 22.6z"/>
        <path class="st126" d="M1178.6 2130.9c0 .1 0 .2-.1.2-1.1 5.3-3.2 3-3.2 3v-.5l.1-2.6.5-9.5s0-.1.1-.3c.2-.3.7-.7 1.5-.4.7.2 1.2.8 1.4 1.6.7 1.7.4 4.5-.3 8.5z"/>
        <path class="st129" d="M1162.1 2103.4v44.3c8-.1 14.1-8.6 14.1-22.6 0-17.5-5.1-21.6-14.1-21.7z"/>
        <path class="st254" d="M1181.7 2105.3s-.4 3.1-3.3 6.1c-.8.8-1.8 1.7-3.1 2.4h-.1c-2.9 1.7-7 2.9-12.8 2.9h-.2c-9.2-.1-11.5-5.6-11.5-5.6s-1.4 2-1.8 8.6c-.1 2-.1 4.3 0 7.2h-1.4s-1.2-2.3-1.9-5.5c-.1-.5-.2-1.1-.3-1.7-.4-3.1-.1-6.7 2.2-9.7 0-3 .3-5.4 3.8-8 8.7-6.5 15.7 1.3 27.4-4.3-.2.3-4.3 5.2-8.2 5.7 0 0 5.5 2.7 12.3-5.7 0 0-.9 8.3-9 12 0 .1 3.6.3 7.9-4.4z"/>
        <path class="st254" d="M1179.6 2119.7c-.1 1-.3 1.9-.6 2.8-.7 2.6-1.6 4.4-1.6 4.4h-1.4c.1-2.1.1-4 0-5.6 0-.4 0-.8-.1-1.2v-.3c-.2-2.7-.5-4.6-.8-5.9-.2-.9-.5-1.6-.6-2-.2-.5-.3-.7-.3-.7h.1l3.1-1.1c.3.5.7.9.9 1.4 1.5 2.6 1.7 5.6 1.3 8.2z"/>
        <path class="st252" d="M1179.1 2122.5c.5 1.6.3 4.4-.5 8.4 0 .1 0 .2-.1.2h-32.9c0-.1 0-.2-.1-.2-1-5-1.1-8.1.1-9.4-.1-.5-.2-1.1-.3-1.7h34.3c-.1.9-.3 1.9-.5 2.7z"/>
        <ellipse class="st253" cx="1155.2" cy="2125.4" rx="3" ry="2.3"/>
        <path class="st255" d="M1162.1 2119.7v11.4h16.4c0-.1 0-.2.1-.2.7-4 1-6.7.5-8.4.2-.8.4-1.8.6-2.8h-17.6z"/>
        <ellipse class="st253" cx="1169.5" cy="2125.4" rx="3" ry="2.3"/>
        <text transform="matrix(.992 0 0 1 1118.274 2207.583)">
          <tspan x="0" y="0" class="st92 st90 st256">Reducing</tspan><tspan x="-25.6" y="24.1" class="st92 st90 st256">Campus Crime</tspan>
        </text>
      </g>
      <g id="evening-icon-2">
        <path class="st130" d="M1336.9 2101.3h6.6v13.6h-6.6z"/>
        <path class="st130" d="M1399.9 2123.5l-37.6-29.9-37.7 29.9z"/>
        <path class="st257" d="M1362.3 2098.5l-31.5 25v46.8h62.9v-46.8z"/>
        <path class="st258" d="M1393.7 2170.3v-46.8l-31.4-25v71.8z"/>
        <path class="st130" d="M1339 2136h18.5v34.4H1339z"/>
        <path class="st259" d="M1366.9 2129.6h18.6v28.5h-18.6z"/>
        <path class="st130" d="M1327.3 2170.3h70v3.9h-70z"/>
        <path class="st260" d="M1389.7 2181.9c8.2 0 17.2-8.4 17.2-35-8.4 0-15.5-2.9-17.2-5.5-1.6 2.6-8.8 5.5-17.2 5.5.1 26.6 9 35 17.2 35z"/>
        <path class="st130" d="M1406.9 2146.9c-8.4 0-15.5-2.9-17.2-5.5v40.5c8.2 0 17.2-8.4 17.2-35z"/>
        <path class="st261" d="M1404.6 2149.2c-.4 20.4-6.2 27.2-10.7 29.4-1.7.8-3.2 1-4.1 1h-.8c-1.3-.1-3.1-.6-5.1-2-1-.7-1.9-1.7-2.9-2.9-.9-1.2-1.8-2.7-2.5-4.6-.6-1.3-1.1-2.7-1.5-4.3-.5-1.8-.9-3.7-1.2-5.9-.2-1.6-.4-3.4-.6-5.3-.1-1.6-.2-3.4-.2-5.3 2.3-.1 4.5-.5 6.4-1 3.7-.9 6.6-2.2 8.4-3.6.2.1.4.3.6.4 2.8 1.8 7.9 3.7 14.2 4.1z"/>
        <path class="st262" d="M1404.6 2149.1c-6.7-.4-12-2.4-14.8-4.5v35c3.3 0 14.2-2.3 14.8-30.5z"/>
        <path class="st263" d="M1390.3 2145l-14.6 14.7c-.2-1.6-.4-3.4-.6-5.3l6.2-6.2c3.7-.9 6.6-2.2 8.4-3.6.2.1.4.3.6.4zm-.6 7.7v5.8l-11.3 11.4c-.6-1.3-1.1-2.7-1.5-4.3l12.8-12.9zm0 13v5.8l-5.9 5.9c-1-.7-1.9-1.7-2.9-2.9l8.8-8.8zm-.7 13.8l.8-.8v.8c-.3.1-.6 0-.8 0z"/>
        <text transform="matrix(.992 0 0 1 1314.583 2207.583)">
          <tspan x="0" y="0" class="st92 st90 st256">Improving</tspan><tspan x="-18.8" y="24.1" class="st92 st90 st256">Overall Safety</tspan>
        </text>
      </g>
      <g id="evening-icon-3">
        <g id="car_1_">
          <g id="XMLID_148_">
            <path id="XMLID_150_" class="st264" d="M1617.3 2174.4h-98.5c-.9 0-1.6-.7-1.6-1.6 0-.9.7-1.6 1.6-1.6h98.5c.9 0 1.6.7 1.6 1.6 0 .8-.7 1.6-1.6 1.6z"/>
          </g>
          <path class="st265" d="M1604.2 2143.2l-.3-2.5c-2.5-1.3-6-2-11.3-2h-7.1c-1.6-7.7-8.4-17-16.5-17h-36.8c-9 0-13.2 6.1-13.5 16v23.6c0 .6 0 1.1.1 1.7h90.5c.1-.6.1-1.1.1-1.7v-7.5c-2.3-3.2-4.1-6.7-5.2-10.6z"/>
          <g id="XMLID_174_">
            <path id="XMLID_180_" class="st266" d="M1562.4 2125.1v16.5h20.3l-.5-2.2c-.7-3.4-2.6-7.1-5-9.8-1.3-1.4-3.6-3.6-6.5-4.3-.5-.1-1.1-.2-1.7-.2h-6.6z"/>
            <path id="XMLID_179_" class="st266" d="M1538.8 2125.1h20.2v16.5h-20.2z"/>
            <path id="XMLID_178_" class="st267" d="M1545 2125.1l7.8 16.5h5.4l-7.8-16.5z"/>
            <path id="XMLID_177_" class="st267" d="M1565.2 2125.1l7.8 16.5h5.4l-7.7-16.3c-.5-.1-1.1-.2-1.7-.2h-3.8z"/>
            <path id="XMLID_176_" class="st266" d="M1522.2 2138.7v2.9h13.2v-16.5h-3.1c-2 0-3.6.3-5 1.1-.9.5-1.7 1.1-2.4 1.9-.5.6-.8 1.2-1.2 1.9-.9 2-1.5 4.6-1.5 7.7v1z"/>
            <path id="XMLID_175_" class="st267" d="M1523.7 2130l5.5 11.6h5.4l-7.3-15.4c-.9.5-1.7 1.1-2.4 1.9-.4.6-.8 1.2-1.2 1.9z"/>
          </g>
          <path id="XMLID_173_" class="st266" d="M1518.3 2166.7h14.5c.8 0 1.4-.6 1.4-1.4v-4.2c0-.8-.6-1.4-1.4-1.4h-14.5c-.8 0-1.4.6-1.4 1.4v4.2c0 .8.6 1.4 1.4 1.4z"/>
          <path id="XMLID_172_" class="st266" d="M1590.35 2165.964h-48.4v-5.9h48.4z"/>
          <g id="XMLID_124_">
            <g id="XMLID_165_">
              <g id="XMLID_169_">
                <path id="XMLID_171_" class="st268" d="M1535.7 2162.9v-10.5h.1c5.7 0 10.3 4.6 10.3 10.4v.1h-10.4z"/>
                <path id="XMLID_170_" class="st266" d="M1535.7 2162.9v-10.5h-.1c-5.7 0-10.3 4.6-10.3 10.4v.1h10.4z"/>
              </g>
              <g id="XMLID_166_">
                <path id="XMLID_168_" class="st268" d="M1535.7 2162.9v10.5h-.1c-5.7 0-10.3-4.6-10.3-10.4v-.1h10.4z"/>
                <path id="XMLID_167_" class="st266" d="M1535.7 2162.9v10.5h.1c5.7 0 10.3-4.6 10.3-10.4v-.1h-10.4z"/>
              </g>
            </g>
            <ellipse id="XMLID_164_" class="st269" cx="1535.7" cy="2162.9" rx="6.6" ry="6.7"/>
            <ellipse id="XMLID_163_" class="st266" cx="1535.7" cy="2162.9" rx="3.1" ry="3.2"/>
          </g>
          <g id="XMLID_82_">
            <g id="XMLID_210_">
              <path id="XMLID_162_" class="st270" d="M1523.5 2157.2c-.1 0-.2 0-.2-.1-.2-.1-.3-.4-.2-.7 2.4-4.8 7.2-7.8 12.6-7.8h.2c2 0 4 .4 5.8 1.3.3.1.4.4.3.7-.1.3-.4.4-.7.3-1.7-.8-3.5-1.2-5.4-1.2h-.1l-.1-.5v.5c-5 0-9.4 2.8-11.7 7.3-.2.1-.3.2-.5.2z"/>
            </g>
            <g id="XMLID_95_">
              <path id="XMLID_161_" class="st270" d="M1548.6 2158.8c-.2 0-.4-.1-.5-.3-.4-1.3-1.1-2.4-1.8-3.5-.2-.2-.1-.5.1-.7.2-.2.5-.1.7.1.8 1.2 1.5 2.4 2 3.8.1.3 0 .6-.3.6h-.2z"/>
            </g>
          </g>
          <g id="XMLID_160_">
            <g id="XMLID_209_">
              <path id="XMLID_211_" class="st270" d="M1578 2157.2c-.1 0-.2 0-.2-.1-.2-.1-.3-.4-.2-.7 2.4-4.8 7.2-7.8 12.6-7.8h.2c2 0 4 .4 5.8 1.3.3.1.4.4.3.7-.1.3-.4.4-.7.3-1.7-.8-3.5-1.2-5.4-1.2h-.1l-.1-.5v.5c-5 0-9.4 2.8-11.7 7.3-.1.1-.3.2-.5.2z"/>
            </g>
          </g>
          <path id="XMLID_122_" class="st266" d="M1595.8 2166.7h14.5c.8 0 1.4-.6 1.4-1.4v-4.2c0-.8-.6-1.4-1.4-1.4h-14.5c-.8 0-1.4.6-1.4 1.4v4.2c.1.8.7 1.4 1.4 1.4z"/>
          <g id="XMLID_109_">
            <g id="XMLID_115_">
              <g id="XMLID_119_">
                <path id="XMLID_121_" class="st268" d="M1590.3 2162.9v-10.5h.1c5.7 0 10.3 4.6 10.3 10.4v.1h-10.4z"/>
                <path id="XMLID_120_" class="st266" d="M1590.3 2162.9v-10.5h-.1c-5.7 0-10.3 4.6-10.3 10.4v.1h10.4z"/>
              </g>
              <g id="XMLID_116_">
                <path id="XMLID_118_" class="st268" d="M1590.3 2162.9v10.5h-.1c-5.7 0-10.3-4.6-10.3-10.4v-.1h10.4z"/>
                <path id="XMLID_117_" class="st266" d="M1590.3 2162.9v10.5h.1c5.7 0 10.3-4.6 10.3-10.4v-.1h-10.4z"/>
              </g>
            </g>
            <ellipse id="XMLID_112_" class="st269" cx="1590.3" cy="2162.9" rx="6.6" ry="6.7"/>
            <ellipse id="XMLID_110_" class="st266" cx="1590.3" cy="2162.9" rx="3.1" ry="3.2"/>
          </g>
          <path id="XMLID_108_" class="st270" d="M1518.8 2149.8c0 .1 0 .1 0 0v4.3h1.9c1.9 0 3.4-1.5 3.4-3.4v-2.8c0-1.9-1.5-3.4-3.4-3.4h-1.9v5.3z"/>
          <g id="XMLID_106_">
            <path id="XMLID_107_" class="st266" d="M1562 2146.4c.1-1.4 1.3-2.5 2.7-2.5h3.8c1.4 0 2.6 1.1 2.7 2.5h-9.2z"/>
          </g>
          <g id="XMLID_102_">
            <path id="XMLID_105_" class="st266" d="M1538.4 2146.4c.1-1.4 1.3-2.5 2.7-2.5h3.8c1.4 0 2.6 1.1 2.7 2.5h-9.2z"/>
          </g>
          <path class="st11" d="M1604.7 2144.6c-1.7.2-3.1 1.6-3.1 3.4v5.3c0 1.9 1.5 3.4 3.4 3.4h2.9c.6 0 1.1-.1 1.6-.4v-2.4c-2.1-2.9-3.7-6-4.8-9.3z"/>
          <path class="st270" d="M1609.3 2153.6h-7.7v1.6c0 1.9 1.5 1.8 3.4 1.8h4.5v-3.2c-.1-.1-.1-.2-.2-.2z"/>
          <g id="smoke">
            <path class="st11" d="M1602.4 2123.8c-1 .6-2.3 1.3-2.3 2.7 0 1.5 1.3 2.2 2.3 2.7.5.3.9.5 1.2.8.1-.5.2-.9.3-1.4-.3-.2-.6-.4-.8-.5-1-.6-1.6-.9-1.6-1.6 0-.6.6-1 1.6-1.6 1-.6 2.3-1.3 2.3-2.7 0-1.5-1.3-2.2-2.3-2.7-1-.6-1.6-.9-1.6-1.6 0-.6.6-1 1.6-1.6 1-.6 2.3-1.3 2.3-2.7 0-.4-.3-.7-.6-.7-.4 0-.6.3-.6.7 0 .6-.6 1-1.6 1.6-1 .6-2.3 1.3-2.3 2.7 0 1.5 1.3 2.2 2.3 2.7 1 .6 1.6.9 1.6 1.6s-.9 1-1.8 1.6z" id="XMLID_194_"/>
            <g id="XMLID_157_">
              <path id="XMLID_271_" class="st11" d="M1594.9 2129.2c-.4 0-.6-.3-.6-.7 0-1-.6-1.4-1.7-2.1-1-.7-2.2-1.5-2.2-3.2 0-1.7 1.2-2.5 2.2-3.2 1-.7 1.7-1.2 1.7-2.1s-.6-1.4-1.7-2.1c-1-.7-2.2-1.5-2.2-3.2 0-1.7 1.2-2.5 2.2-3.2 1-.7 1.7-1.2 1.7-2.1 0-.4.3-.7.6-.7.4 0 .6.3.6.7 0 1.7-1.2 2.5-2.2 3.2-1 .7-1.7 1.2-1.7 2.1s.6 1.4 1.7 2.1c1 .7 2.2 1.5 2.2 3.2 0 1.7-1.2 2.5-2.2 3.2-1 .7-1.7 1.2-1.7 2.1s.6 1.4 1.7 2.1c1 .7 2.2 1.5 2.2 3.2.1.4-.2.7-.6.7z"/>
            </g>
          </g>
        </g>
        <path class="st11" d="M1604.4 2135.5s.1 0 .3-.1c.1 0 .2-.1.3-.1.1 0 .3-.1.4 0 .3 0 .7.1 1 .2.3.2.7.4 1 .7.3.3.5.7.7 1 .2.3.2.7.3 1v.7c0 .2-.1.3-.1.3v-.3c0-.2-.1-.4-.1-.7-.2-.5-.5-1.2-1-1.8-.2-.3-.5-.5-.8-.7-.3-.2-.6-.3-.9-.3h-.7c-.3.1-.4.1-.4.1zm-.5-1.7s.1-.1.3-.2c.1-.1.2-.1.4-.2s.3-.2.5-.2c.4-.1.9-.1 1.4 0 .5.1 1 .3 1.5.6s.9.7 1.2 1.1c.3.4.6.8.7 1.2.1.2.2.4.2.5 0 .2.1.3.1.4v.4s0-.1-.1-.4c0-.1-.1-.2-.1-.4-.1-.1-.2-.3-.2-.5-.4-.7-1.1-1.5-1.9-2-.4-.3-.9-.5-1.3-.6-.5-.1-.9-.2-1.3-.1-.2 0-.4.1-.5.1-.2 0-.3.1-.4.1-.4.2-.5.2-.5.2zm6.4 14.6h.6c.1 0 .3 0 .4.1.3.1.6.3.9.6.3.3.5.6.6 1l.3 1.2c0 .4 0 .7-.1 1-.1.3-.2.5-.3.7l-.2.2s0-.1.1-.3c.1-.2.1-.4.1-.7 0-.6 0-1.3-.3-2-.1-.4-.3-.7-.5-.9-.2-.3-.5-.5-.7-.6-.1-.1-.2-.1-.3-.2-.1-.1-.2-.1-.3-.1-.2.1-.3 0-.3 0zm0-1.7s.1 0 .4-.1c.1 0 .3-.1.4-.1h.6c.4.1.9.2 1.3.5.2.1.4.3.6.5.2.2.4.4.5.6.3.5.6.9.7 1.4.2.5.2 1 .3 1.4v.6c0 .2 0 .3-.1.4-.1.2-.1.4-.1.4v-.8c0-.2 0-.3-.1-.5-.1-.8-.5-1.8-1.1-2.6-.1-.2-.3-.4-.5-.6-.2-.2-.4-.3-.6-.5-.4-.3-.8-.5-1.2-.6-.2-.1-.4-.1-.5-.1h-.4c0 .1-.2.1-.2.1z"/>
        <text transform="matrix(.992 0 0 1 1522.464 2209.845)">
          <tspan x="0" y="0" class="st92 st90 st256">Reducing</tspan><tspan x="-22" y="24.1" class="st92 st90 st256">Drunk Driving</tspan>
        </text>
      </g>
    </g>
    <g id="social-responsibility">
      <text transform="translate(193.404 2422.486)" class="st89 st90 st91">
        Social Responsibility
      </text>
      <text transform="translate(193.404 2460.935)">
        <tspan x="0" y="0" class="st92 st93 st165">We believe in giving back to the community – with our model we expect</tspan><tspan x="0" y="24.5" class="st92 st93 st165">to donate a percentage of the revenue every two years back to the </tspan><tspan x="0" y="49" class="st92 st93 st165">university to go towards campus beautification, research and development</tspan><tspan x="0" y="73.4" class="st92 st93 st165">and scholarships.</tspan>
      </text>
      <g id="social-icon-3">
        <path class="st271" d="M525.6 2675.5h25.8v-43l-12.9-8.3-12.9 8.3v43zm-53.9 0h25.8v-33l-12.9-8.3-12.9 8.3v33z"/>
        <path class="st272" d="M483.2 2664.4h2.9v5.5h-2.9v-5.5zm0-10h2.9v5.4h-2.9v-5.4zm0-10h2.9v5.4h-2.9v-5.4z"/>
        <path class="st273" d="M496.4 2675.5h27.4v-78h-27.4v78z"/>
        <path class="st274" d="M527.5 2611.2v-3.1c.1-.1.2-.3.2-.6h.2v4.2h-.2c0-.2-.1-.3-.2-.5zm-5.4.5v-4.2h.2c0 .2.1.4.2.6v3.1c-.1.1-.2.3-.2.5h-.2z"/>
        <path class="st275" d="M508 2664.4h2.8v5.5H508v-5.5z"/>
        <path class="st276" d="M517.6 2664.4h2.9v5.5h-2.9v-5.5zm-13 8.2h28.9v2.9h-28.9v-2.9z"/>
        <path class="st277" d="M504.6 2662.6h9.6v10h-9.6v-10zm3.4 1.8h2.9v5.5H508v-5.5z"/>
        <path class="st278" d="M514.2 2662.6h9.6v10h-9.6v-10zm3.4 1.8h2.9v5.5h-2.9v-5.5z"/>
        <path class="st279" d="M523.8 2662.6h9.6v10h-9.6v-10zm3.4 1.8h2.9v5.5h-2.9v-5.5z"/>
        <path class="st280" d="M504.6 2652.5h9.6v10h-9.6v-10zm3.4 1.9h2.9v5.5H508v-5.5z"/>
        <path class="st277" d="M514.2 2652.5h9.6v10h-9.6v-10zm3.4 1.9h2.9v5.5h-2.9v-5.5z"/>
        <path class="st278" d="M523.8 2652.5h9.6v10h-9.6v-10zm3.4 1.9h2.9v5.5h-2.9v-5.5z"/>
        <path class="st281" d="M504.6 2642.5h9.6v10h-9.6v-10zm3.4 1.9h2.9v5.5H508v-5.5z"/>
        <path class="st280" d="M514.2 2642.5h9.6v10h-9.6v-10zm3.4 1.9h2.9v5.5h-2.9v-5.5z"/>
        <path class="st277" d="M523.8 2642.5h9.6v10h-9.6v-10zm3.4 1.9h2.9v5.5h-2.9v-5.5z"/>
        <path class="st282" d="M523.8 2632.5h9.6v10h-19.2v-10h9.6zm-6.2 1.8h2.9v5.5h-2.9v-5.5zm9.6 0h2.9v5.5h-2.9v-5.5z"/>
        <path class="st283" d="M504.6 2632.5h9.6v10h-.8v-8.6h-8v8.6h-.8v-10zm19.2-10.1h9.7v10.1h-.9v-8.6h-7.9v8.6H523v-8.6h-8v8.6h-.8v-10.1h9.6z"/>
        <path class="st284" d="M527.2 2664.4h2.9v5.5h-2.9v-5.5z"/>
        <path class="st285" d="M508 2654.4h2.8v5.5H508v-5.5z"/>
        <path class="st275" d="M517.6 2654.4h2.9v5.5h-2.9v-5.5z"/>
        <path class="st276" d="M527.2 2654.4h2.9v5.5h-2.9v-5.5z"/>
        <path class="st286" d="M508 2644.4h2.8v5.4H508v-5.4z"/>
        <path class="st285" d="M517.6 2644.4h2.9v5.4h-2.9v-5.4z"/>
        <path class="st275" d="M527.2 2644.4h2.9v5.4h-2.9v-5.4z"/>
        <path class="st287" d="M581.2 2675.5c1 0 1.7.8 1.7 1.7 0 1-.8 1.7-1.7 1.7H464.3c-1 0-1.7-.8-1.7-1.7 0-1 .8-1.7 1.7-1.7h116.9z"/>
        <path class="st288" d="M509.7 2678h28.5c.5 0 .9.4.9.9s-.4.9-.9.9h-28.5c-.5 0-.9-.4-.9-.9s.4-.9.9-.9z"/>
        <path class="st289" d="M477.1 2677.3h25.7c.9 0 1.6.7 1.6 1.6s-.7 1.6-1.6 1.6h-25.7c-.9 0-1.6-.7-1.6-1.6s.7-1.6 1.6-1.6z"/>
        <path class="st280" d="M521.4 2600.5c.8 0 1.4.6 1.4 1.4s-.6 1.4-1.4 1.4-1.4-.6-1.4-1.4.6-1.4 1.4-1.4zm-53 4c.8 0 1.4.6 1.4 1.4s-.6 1.4-1.4 1.4-1.4-.6-1.4-1.4.6-1.4 1.4-1.4zm19.2-15.9c.8 0 1.4.6 1.4 1.4s-.6 1.4-1.4 1.4-1.4-.6-1.4-1.4.7-1.4 1.4-1.4z"/>
        <path class="st290" d="M487.2 2669.4c0-.1 0-.2.1-.3l4.4-5.3h-4.1c-.2 0-.4-.2-.4-.4 0-.1 0-.2.1-.3l4.4-5.3h-4.1c-.2 0-.4-.2-.4-.4 0-.1 0-.2.1-.3l4.4-5.3h-4.1c-.2 0-.4-.2-.4-.4 0-.1 0-.2.1-.3l4.4-5.3h-4.1c-.2 0-.4-.2-.4-.4 0-.1 0-.2.1-.3l4.4-5.3h-4.1c-.2 0-.4-.2-.4-.4 0-.1 0-.2.1-.3l4.4-5.3h-4.1c-.2 0-.4-.2-.4-.4v-.1c0-.1 0-.3.1-.4l4.4-5.3h-4.1c-.2 0-.4-.2-.4-.4 0-.1 0-.2.1-.3l4.4-5.3h-4.1c-.2 0-.4-.2-.4-.4 0-.1 0-.2.1-.3l5-6c.2-.2.4-.2.6-.1.2.2.2.4.1.6l-4.4 5.3h4.1c.2 0 .4.2.4.4 0 .1 0 .2-.1.3l-4.4 5.3h4.1c.2 0 .4.2.4.4 0 .1 0 .2-.1.3l-4.6 5.5h4.3c.2 0 .4.2.4.4 0 .1 0 .2-.1.3l-4.4 5.3h4.1c.2 0 .4.2.4.4 0 .1 0 .2-.1.3l-4.4 5.3h4.1c.2 0 .4.2.4.4 0 .1 0 .2-.1.3l-4.4 5.3h4.1c.2 0 .4.2.4.4 0 .1 0 .2-.1.3l-4.4 5.3h4.1c.2 0 .4.2.4.4 0 .1 0 .2-.1.3l-4.4 5.3h4.1c.2 0 .4.2.4.4 0 .1 0 .2-.1.3l-4.4 5.3h4.1c.2 0 .4.2.4.4h-5.9v.1zm41.8-63.5c0 .2-.2.4-.4.4s-.4-.2-.4-.4v-3.3l-6.5 3.7c-.1 0-.2.1-.2.1-.2 0-.4-.2-.4-.4v-3.3l-6.5 3.7c-.1 0-.2.1-.2.1-.2 0-.4-.2-.4-.4v-3.3l-6.5 3.7c-.1 0-.2.1-.2.1-.2 0-.4-.2-.4-.4v-3.3l-6.5 3.7c-.1 0-.2.1-.2.1-.2 0-.4-.2-.4-.4v-4.1c0-.2.2-.4.4-.4s.4.2.4.4v3.3l6.5-3.7c.1 0 .2-.1.2-.1.2 0 .4.2.4.4v3.3l6.5-3.7c.1 0 .2-.1.2-.1.2 0 .4.2.4.4v3.3l6.5-3.7c.1 0 .2-.1.2-.1.2 0 .4.2.4.4v3.3l6.5-3.7c.1 0 .2-.1.2-.1.2 0 .4.2.4.4v4.1zm-36-.3c.2.2.1.5-.1.6-.2.2-.5.1-.6-.1l-5-6c-.1-.1-.1-.2-.1-.3 0-.2.2-.4.4-.4h3.1c.2 0 .4.2.4.4s-.2.4-.4.4h-2.2l4.5 5.4zm-19.5-4.1l6.5 3.7v-3.3c0-.2.2-.4.4-.4s.4.2.4.4v4.1c0 .2-.2.4-.4.4-.1 0-.2 0-.2-.1l-6.5-3.7v3.3c0 .2-.2.4-.4.4s-.4-.2-.4-.4v-4.1c0-.2.2-.4.4-.4.1 0 .2 0 .2.1z"/>
        <path class="st291" d="M492.2 2669.4v-63h-4.1v63h-.9v-79.5c0-.3.2-.5.5-.5.2 0 .4.1.4.3l4.9 15.6h.1v64h-.9v.1zm-4.1-63.9h3.9l-3.9-12.5v12.5z"/>
        <path class="st291" d="M499.6 2601.5c.1 0 .2-.1.3-.1h28.7c.1 0 .2 0 .3.1l7.1 4c.2.1.3.2.3.4 0 .3-.2.5-.5.5H491l1.5-.9 7.1-4zm28.9.8H500l-5.6 3.1H534l-5.5-3.1zm-60.4 3.3l4.9-4c.1-.1.2-.1.3-.1h7.2c.1 0 .2 0 .3.1l7.1 4c.2.1.3.2.3.4 0 .3-.2.5-.5.5h-19.3c-.3 0-.5-.2-.5-.5 0-.2.1-.4.2-.4zm17.8-.1l-5.6-3.1h-6.9l-3.8 3.1h16.3z"/>
        <path class="st292" d="M494.4 2615h-6c-.4 0-.7-.3-.7-.7v-7.6c0-.4.3-.7.7-.7h6c.4 0 .7.3.7.7v7.6c.1.3-.3.7-.7.7z"/>
        <path class="st274" d="M467.6 2604.8l19.1-15.8c-.2.2-.4.6-.4.9l-17.7 14.7h-.2c-.3-.1-.6 0-.8.2zm20.6-16.1l33.5 11.8h-.3c-.2 0-.5.1-.6.2l-31.8-11.2c-.2-.4-.5-.7-.8-.8z"/>
        <path class="st293" d="M472.8 2610.4h4.1v-4h-4.1v4zm12.3 59h10.1v6.1h-10.1v-6.1z"/>
        <path class="st294" d="M476.9 2610.4h4v-4h-4v4z"/>
        <path class="st295" d="M494.4 2615h-2.2v-9h2.2c.4 0 .7.3.7.7v7.6c.1.3-.3.7-.7.7z"/>
        <path class="st296" d="M495.2 2612.5h-4.3c-.2 0-.4-.2-.4-.4v-4.3c0-.2.2-.4.4-.4h4.3v5.1z"/>
        <path class="st292" d="M495.2 2612.5h-3v-5.1h3v5.1z"/>
        <path class="st280" d="M521.8 2613.1l3.2 1.3v-2.7h-3.2v1.4z"/>
        <path class="st279" d="M525.8 2614c.3.2.5.6.5 1 0 .7-.6 1.3-1.3 1.3-.7 0-1.3-.6-1.3-1.3h.7c0 .4.3.7.7.7.4 0 .7-.3.7-.7 0-.4-.3-.7-.7-.7l.7-.3z"/>
        <path class="st297" d="M521 2607.6h4v-1.2h-4v1.2z"/>
        <path class="st278" d="M528.1 2613.1l-3.1 1.3v-2.7h3.1v1.4z"/>
        <path class="st294" d="M525 2607.6h4v-1.2h-4v1.2z"/>
        <path class="st280" d="M523.1 2611c.4 0 .8.4.8.8h-1.6c0-.5.4-.8.8-.8zm3.8 0c.4 0 .8.4.8.8h-1.6c0-.5.3-.8.8-.8zm-3-3.4c0 .4-.4.8-.8.8s-.8-.4-.8-.8h1.6zm3.8 0c0 .4-.4.8-.8.8s-.8-.4-.8-.8h1.6z"/>
        <path class="st279" d="M523.1 2607.2c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4.2-.4.4-.4zm0 4.2c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4c0-.3.2-.4.4-.4zm3.8-4.2c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4.1-.4.4-.4zm0 4.2c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4c0-.3.1-.4.4-.4z"/>
        <path class="st298" d="M531.8 2622.4v1.5h-3.4v-.9h-2.8v.9h-.9v7.3H523v-8.8h8.8z"/>
        <path class="st282" d="M520.2 2619.1h9.6v10h-9.6v-10zm3.3 1.9h2.9v5.5h-2.9v-5.5z"/>
        <path class="st274" d="M520.3 2619.3c-.1.1-.2.1-.3 0-.1-.1-.1-.2 0-.3l4.8-3.7c.1-.1.2-.1.3 0 .1.1.1.2 0 .3l-4.8 3.7z"/>
        <path class="st274" d="M524.9 2615.6c-.1-.1-.1-.2 0-.3.1-.1.2-.1.3 0l4.8 3.7c.1.1.1.2 0 .3-.1.1-.2.1-.3 0l-4.8-3.7z"/>
        <path class="st299" d="M468.2 2666.2v9.2h-.4v-8.8c0-.2.2-.4.4-.4z"/>
        <path class="st300" d="M468.2 2666.2c.2 0 .4.2.4.4v8.8h-.4v-9.2z"/>
        <path class="st299" d="M477.1 2666.2v9.2h-.4v-8.8c-.1-.2.1-.4.4-.4z"/>
        <path class="st300" d="M477.1 2666.2c.2 0 .4.2.4.4v8.8h-.4v-9.2z"/>
        <path class="st301" d="M478.4 2667.7v2.6c0 .3-.3.6-.6.6h-1.3l1.8-3.5s.1.1.1.3z"/>
        <path class="st283" d="M478.3 2667.3l-1.8 3.5h-1.9l1.9-3.7h1.3c.2 0 .3.1.5.2z"/>
        <path class="st301" d="M476.5 2667.1l-1.9 3.7h-1.9l1.9-3.7h1.9z"/>
        <path class="st283" d="M472.7 2667.1h1.9l-1.9 3.7h-2l2-3.7z"/>
        <path class="st301" d="M470.7 2667.1h2l-2 3.7h-1.9l1.9-3.7z"/>
        <path class="st283" d="M468.8 2667.1h1.9l-1.9 3.7h-1.3c-.2 0-.4-.1-.5-.2l1.8-3.5z"/>
        <path class="st301" d="M466.9 2670.2v-2.6c0-.3.3-.6.6-.6h1.3l-1.8 3.5s-.1-.1-.1-.3z"/>
        <path class="st299" d="M477.1 2673.7h-8.8c0-.2.2-.4.4-.4h7.9c.3 0 .5.2.5.4z"/>
        <path class="st300" d="M477.1 2673.7c0 .2-.2.4-.4.4h-7.9c-.2 0-.4-.2-.4-.4h8.7z"/>
        <path class="st302" d="M537 2664.4h2.9v5.5H537v-5.5zm0-10h2.9v5.4H537v-5.4zm0-10h2.9v5.4H537v-5.4z"/>
        <path class="st299" d="M539.5 2666.2v9.2h-.4v-8.8c0-.2.2-.4.4-.4z"/>
        <path class="st300" d="M539.5 2666.2c.2 0 .4.2.4.4v8.8h-.4v-9.2z"/>
        <path class="st299" d="M548.4 2666.2v9.2h-.4v-8.8c-.1-.2.1-.4.4-.4z"/>
        <path class="st300" d="M548.4 2666.2c.2 0 .4.2.4.4v8.8h-.4v-9.2z"/>
        <path class="st301" d="M549.7 2667.7v2.6c0 .3-.3.6-.6.6h-1.3l1.8-3.5s.1.1.1.3z"/>
        <path class="st283" d="M549.5 2667.3l-1.8 3.5h-1.9l1.9-3.7h1.3c.3 0 .4.1.5.2z"/>
        <path class="st301" d="M547.8 2667.1l-1.9 3.7h-2l2-3.7h1.9z"/>
        <path class="st283" d="M543.9 2667.1h2l-2 3.7H542l1.9-3.7z"/>
        <path class="st301" d="M542 2667.1h1.9l-1.9 3.7h-1.9l1.9-3.7z"/>
        <path class="st283" d="M540.1 2667.1h1.9l-1.9 3.7h-1.3c-.2 0-.4-.1-.5-.2l1.8-3.5z"/>
        <path class="st301" d="M538.2 2670.2v-2.6c0-.3.3-.6.6-.6h1.3l-1.8 3.5s-.1-.1-.1-.3z"/>
        <path class="st299" d="M548.4 2673.7h-8.8c0-.2.2-.4.4-.4h7.9c.3 0 .5.2.5.4z"/>
        <path class="st300" d="M548.4 2673.7c0 .2-.2.4-.4.4h-8c-.2 0-.4-.2-.4-.4h8.8z"/>
        <path class="st302" d="M537 2634.3h2.9v5.5H537v-5.5z"/>
        <path class="st303" d="M568.3 2603.9c.7.5 1 1.3 1.1 2.3 1.4-1.1 3-1.3 4.1-.5 1.3 1 1.2 3.5-.3 5.4-1 1.3-2.5 2.1-3.7 2.1h-6.1c-.7 0-1.4-.2-1.9-.6-.5-.4-.8-.9-1-1.6-.1.2-.2.4-.4.5-1.2 1.5-3 2.1-4 1.3s-.9-2.7.3-4.2 3-2.1 4-1.3c.2.1.3.3.4.5.3-.6.6-1.3 1.1-1.9 1.9-2.4 4.8-3.3 6.4-2zm8.4 6.2c.8.6.9 1.7.3 2.4-.6.7-1.7.9-2.4.3-.8-.6-.9-1.7-.3-2.4.6-.7 1.7-.9 2.4-.3zm-24.2-12.5c1.1.9 1.3 2.5.8 4.2.7-.4 1.5-.4 2 0 .8.6.7 2.1-.2 3.3-.9 1.2-2.3 1.6-3.2 1-.4-.3-.6-.8-.6-1.3-1.1 1-2.4 1.6-3.5 1.6h-6c-.4 0-.7-.1-1-.4-1-.8-.9-2.6.3-4 1.1-1.4 2.8-2 3.8-1.2.2.1.3.3.4.4.2-.6.6-1.2 1.1-1.8 1.8-2.2 4.5-3.1 6.1-1.8z"/>
        <path class="st304" d="M528.9 2678.9c.5 0 .9.4.9.9s-.4.9-.9.9H519c-.5 0-.9-.4-.9-.9s.4-.9.9-.9h9.9zm5.6 0c.5 0 .9.4.9.9s-.4.9-.9.9H532c-.5 0-.9-.4-.9-.9s.4-.9.9-.9h2.5z"/>
        <path class="st288" d="M487.2 2675.5c2.6-4.8 7.6-7.4 11.4-7.4v7.4h-11.4z"/>
        <path class="st304" d="M509.9 2675.5c-2.6-4.8-7.6-7.4-11.4-7.4v7.4h11.4zm-14.5-3.4c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4.2-.4.4-.4zm-2.1-1.2c.1 0 .2.1.2.2s-.1.2-.2.2-.2-.1-.2-.2.1-.2.2-.2zm3.3 2.9c.3 0 .5.2.5.5s-.2.5-.5.5-.5-.2-.5-.5.2-.5.5-.5zm-4.1.1c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4c.1-.2.2-.4.4-.4z"/>
        <path class="st288" d="M500.2 2673.2c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4.2-.4.4-.4zm1.5.8c.1 0 .2.1.2.2s-.1.2-.2.2-.2-.1-.2-.2.1-.2.2-.2z"/>
        <path class="st304" d="M493.1 2673.2c.1 0 .2.1.2.2s-.1.2-.2.2-.2-.1-.2-.2.1-.2.2-.2zm1.7.8c.1 0 .2.1.2.2s-.1.2-.2.2-.2-.1-.2-.2.1-.2.2-.2zm-4.4-.5c.1 0 .2.1.2.2s-.1.2-.2.2-.2-.1-.2-.2.1-.2.2-.2z"/>
        <path class="st305" d="M528 2647.6l-.2 1.4c.1.1.1.1.1.2.2.4 0 .8-.4 1-.4.2-.8 0-1-.4h-6.4l2-3.7c.8-1.2 2.3-1.4 3.4-.4l.8 1.1.6-.1c.1-.1.2-.1.3-.2.4-.2.8 0 1 .4 0 .2 0 .5-.2.7z"/>
        <path class="st306" d="M519.1 2651l1.5-2.8h.3l-.8 1.6h.8l-.8.9-1 .3z"/>
        <path class="st307" d="M532.1 2644l-1 .6c.1.1.2.2.3.4 0 .1 0 .2.1.2l1-.6-.4-.6z"/>
        <path class="st308" d="M528.2 2647l1.8-1 .1-.3c-.1-.1-.1-.1-.1-.2s0-.2-.1-.2l-2.1 1.2c.1.1.2.2.3.4.1 0 .1 0 .1.1z"/>
        <path class="st307" d="M546.4 2641.1l2.2 1.7.4-.5-2.2-1.7c-.1.2-.2.3-.3.4 0 .1 0 .1-.1.1z"/>
        <path class="st308" d="M542.2 2644.3l-14.4 5.6c.1-.2.2-.5.1-.7 0-.1-.1-.2-.1-.2l.1-.6 1.6-1-.1.3c-.1 0-.2 0-.2.1-.4.2-.6.6-.4 1 .2.4.6.6 1 .4s.6-.6.4-1c0-.1-.1-.2-.1-.2l.5-1.2 7.7-4.8 4-2.5 2.8.1c-.4.4-.4 1.1 0 1.6.2.2.5.3.7.3l-2.1 1.9-.9-.4c-.3-.2-.7-.1-.9.1-.3.3-.3.8 0 1.1.1.1.1.1.2.1h.1z"/>
        <path class="st309" d="M561.3 2659.4l5-.3c.6 0 .9.3 1 .7v.2l-7 .2.1-.2c.1-.3.4-.5.9-.6z"/>
        <path class="st310" d="M561.4 2670.5h7.7v-.6h-7.7v.6z"/>
        <path class="st311" d="M579.3 2668.7v.4c0 .4-.3.8-.8.8H560c-.4 0-.7-.3-.8-.8v-.4h20.1z"/>
        <path class="st308" d="M568 2664h9.7c.8 0 1.2.5 1.3 1.4l.3 2.4v.9H568v-4.7z"/>
        <path class="st306" d="M573.9 2664.6h3.3c.2 0 .4.2.4.4l.2 2.3c0 .2-.2.4-.4.4h-4.7l1.2-3.1z"/>
        <path class="st312" d="M570.2 2664h4l-1.8 4.7h-3.9l1.7-4.7z"/>
        <path class="st309" d="M572.3 2664.6h1.6l-1.1 3.1h-.5c-.2 0-.4-.2-.4-.4v-2.3c0-.2.2-.4.4-.4zm-2.3-1.8h.9v1.2h-.9v-1.2z"/>
        <path class="st306" d="M569.6 2662.8v-.5h1.6v.5h-1.6z"/>
        <path class="st309" d="M571.2 2662.3c0-.3-.4-.6-.8-.6s-.8.3-.8.6h1.6z"/>
        <path class="st313" d="M560.3 2660.3h-1l.1 3.6c.2-1.2.5-2.4.9-3.6z"/>
        <path class="st314" d="M560.1 2660.2l-.3-6.6c-.2.1-.5.1-.7 0l.3 6.6h.7z"/>
        <path class="st312" d="M542.7 2642.8l15.2 7.1c4 1.9 5.7 5.1 6.1 8.7l.1.7-2.8.2c-.3-.8-.7-1.5-1.3-2.3l-.1-3.6c.1-.1.3-.1.4-.2.5-.4.5-1.1.1-1.6s-1.1-.5-1.6-.1-.5 1.1-.1 1.6c.2.2.3.3.5.3l.1 2.6c-1.4-1.6-3.2-3-4.9-4.1l-12.5-8c-.1 0-.1-.1-.2-.1-.3-.3-.3-.8 0-1.1.3-.2.7-.3 1-.1zm-.1 1c-.2.2-.5.2-.7 0s-.2-.5 0-.7c.2-.2.5-.2.7 0 .2.2.2.5 0 .7z"/>
        <path class="st313" d="M548.6 2643l6.7 5 .3-.4.1-.1c.1-.1.2-.2.3-.2l-6.8-5.1-.6.8z"/>
        <path class="st308" d="M557 2647.5c0 .1.1.1 0 0l3.3 3.9c-.7-.6-1.5-1.1-2.4-1.5l-3-1.4.7-.9.1-.1c.4-.4 1-.3 1.3 0zm-.3.3c.2.2.2.5 0 .7s-.5.2-.7 0c-.2-.2-.2-.5 0-.7.2-.2.5-.2.7 0z"/>
        <path class="st311" d="M530 2645.5c-.2-.4 0-.8.4-1 .4-.2.8 0 1 .4.2.4 0 .8-.4 1-.4.2-.8 0-1-.4zm.4-.2c-.1-.2 0-.4.2-.5.2-.1.4 0 .5.2.1.2 0 .4-.2.5s-.5 0-.5-.2z"/>
        <path class="st313" d="M537.3 2640.9l-5.2 3 .5.9 5-2.9-.2-.5v-.1c-.1-.2-.1-.3-.1-.4z"/>
        <path class="st312" d="M537.3 2641.4c0-.1 0-.1 0 0-.1-.4-.1-.7.2-.9.1-.1.2-.2.4-.2l4.3-.9-4.5 2.8-.4-.8zm1.1 0c-.2.2-.5.2-.7 0s-.2-.5 0-.7c.2-.2.5-.2.7 0 .2.2.2.5 0 .7zm-8.5 6.5l.8-2c-.2 0-.5-.1-.6-.3l-.8 2c.2.1.5.2.6.3z"/>
        <path class="st306" d="M527 2646.9c.1-.3.4-.4.7-.3s.4.4.3.7-.4.4-.7.3c-.3-.2-.4-.5-.3-.7zm-.2 2.4c.1-.3.4-.4.7-.3.3.1.4.4.3.7s-.4.4-.7.3c-.3-.2-.5-.5-.3-.7z"/>
        <path class="st311" d="M560.3 2651.7c.4.5.4 1.2-.1 1.6-.5.4-1.2.4-1.6-.1-.4-.5-.4-1.2.1-1.6.4-.3 1.2-.3 1.6.1zm-.5.5c.2.2.2.5 0 .7s-.5.2-.7 0c-.2-.2-.2-.5 0-.7.2-.2.5-.2.7 0z"/>
        <path class="st312" d="M559.8 2652.2c.2.2.2.5 0 .7-.2.2-.5.2-.7 0-.2-.2-.2-.5 0-.7.2-.2.5-.2.7 0z"/>
        <path class="st311" d="M556.7 2647.8c.2.2.2.5 0 .7s-.5.2-.7 0c-.2-.2-.2-.5 0-.7.2-.2.5-.2.7 0zm-14.1-4c-.2.2-.5.2-.7 0s-.2-.5 0-.7c.2-.2.5-.2.7 0 .2.2.2.5 0 .7zm4-2.8c-.5.4-1.2.4-1.6 0-.4-.5-.4-1.2 0-1.6.5-.4 1.2-.4 1.6 0 .4.5.4 1.2 0 1.6zm-.5-1.1c.2.2.2.5 0 .7s-.5.2-.7 0c-.2-.2-.2-.5 0-.7s.6-.2.7 0z"/>
        <path class="st312" d="M546.1 2639.9c.2.2.2.5 0 .7s-.5.2-.7 0c-.2-.2-.2-.5 0-.7.2-.2.6-.2.7 0z"/>
        <path class="st311" d="M538.4 2641.4c-.2.2-.5.2-.7 0s-.2-.5 0-.7c.2-.2.5-.2.7 0 .2.2.2.5 0 .7z"/>
        <path class="st312" d="M530.4 2645.3c-.1-.2 0-.4.2-.5.2-.1.4 0 .5.2.1.2 0 .4-.2.5-.3.1-.5 0-.5-.2z"/>
        <path class="st311" d="M528.6 2648.7c-.2-.4 0-.8.4-1 .4-.2.8 0 1 .4.2.4 0 .8-.4 1s-.8 0-1-.4zm1 0c-.1.1-.4.1-.5 0-.1-.1-.1-.4 0-.5.1-.1.4-.1.5 0 .1.1.1.4 0 .5z"/>
        <path class="st312" d="M529.6 2648.7c-.1.1-.4.1-.5 0-.1-.1-.1-.4 0-.5.1-.1.4-.1.5 0 .1.1.1.4 0 .5z"/>
        <path class="st315" d="M564.7 2668.7h-5.5c-.1-1-.1-1.9-.1-2.9l7-1.4c-.9.2-1.4.7-1.4 1.4v2.9zm3.3-4.7z"/>
        <path class="st316" d="M559.2 2665.8c0-1.6.5-3.5 1.1-5.5l7-.2.7 3.9-8.8 1.8z"/>
        <path class="st317" d="M562.8 2660.2h1.5l-1.8 4.9-1.6.3 1.9-5.2z"/>
        <path class="st318" d="M561.8 2660.2h.6l-1.9 5.3-.7.1 2-5.4z"/>
        <path class="st319" d="M559.7 2668.7h1.5l1.3-3.6-1.6.3-1.2 3.3z"/>
        <path class="st320" d="M559.2 2668.7l1.3-3.2h-.2l-.5.1-.6 1.8v1.3z"/>
        <path class="st312" d="M568 2668.7h-3.3l.1-2.9c0-.8.5-1.3 1.4-1.4l1.9-.4v4.7h-.1z"/>
        <path class="st321" d="M555.1 2675.5zm-.2-4.4l6.7-.7h7.3l6.7.7c1.1.1 2 1 2 2.2 0 1.2-1 2.2-2.2 2.2h-20.3c-1.2 0-2.2-1-2.2-2.2 0-1.2.9-2.1 2-2.2z"/>
        <path class="st309" d="M555.1 2675.5c-1.2 0-2.2-1-2.2-2.2 0-1.1.9-2.1 2-2.2l6.7-.7h7.3l6.7.7c1.1.1 2 1 2 2.2 0 1.2-1 2.2-2.2 2.2h-20.3zm20.3-.7c.9 0 1.5-.7 1.5-1.5s-.6-1.5-1.4-1.5l-6.7-.7h-7.2l-6.7.7c-.8.1-1.4.7-1.4 1.5 0 .9.7 1.5 1.5 1.5h20.4z"/>
        <path class="st322" d="M568.9 2671.1c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.2-.6.6-.6zm-3.7 2.5c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.3-.6.6-.6zm2 0c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6c-.1-.3.2-.6.6-.6zm-5.6-2.5c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.3-.6.6-.6zm7.5 2.5c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.2-.6.6-.6zm1.9 0c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.3-.6.6-.6zm1.9 0c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.3-.6.6-.6zm-15.3 0c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.2-.6.6-.6zm1.9 0c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.3-.6.6-.6zm1.9 0c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.3-.6.6-.6zm1.9 0c.3 0 .6.3.6.6s-.3.6-.6.6-.6-.3-.6-.6.3-.6.6-.6zm-8.2-1.6c.7 0 1.3.6 1.3 1.3s-.6 1.3-1.3 1.3-1.3-.6-1.3-1.3.6-1.3 1.3-1.3zm20.3 0c.7 0 1.3.6 1.3 1.3s-.6 1.3-1.3 1.3-1.3-.6-1.3-1.3.6-1.3 1.3-1.3z"/>
        <path class="st323" d="M575.7 2672.4c.4.1.6.5.6.9 0 .5-.4.9-.9.9-.1 0-.2 0-.3-.1l.6-1.7z"/>
        <path class="st324" d="M556.1 2674.1h10.4l.7-2h-11.6c.4.2.7.7.7 1.2.1.3 0 .6-.2.8zm19.3-1.8c.1 0 .2 0 .3.1l-.6 1.7c-.4-.1-.6-.5-.6-.9s.4-.9.9-.9z"/>
        <path class="st323" d="M555.4 2672.4c.4.1.6.5.6.9 0 .5-.4.9-.9.9-.1 0-.2 0-.3-.1l.6-1.7z"/>
        <path class="st324" d="M555.1 2672.3c.1 0 .2 0 .3.1l-.6 1.7c-.4-.1-.6-.5-.6-.9s.4-.9.9-.9z"/>
        <path class="st323" d="M566.5 2674.1h7.9c-.2-.2-.3-.5-.3-.8 0-.5.3-1 .7-1.2h-7.6l-.7 2z"/>
        <path class="st312" d="M537.8 2646l-7.1 2.8 1-2.9 6.4-4 1.6-.9-1.9 5z"/>
        <path class="st271" d="M573.2 2657.8c.8 0 1.5.7 1.5 1.5s-.7 1.5-1.5 1.5-1.5-.7-1.5-1.5c0-.9.6-1.5 1.5-1.5z"/>
        <path class="st271" d="M571.3 2655c1 0 1.8.8 1.8 1.8s-.8 1.8-1.8 1.8-1.8-.8-1.8-1.8.8-1.8 1.8-1.8z"/>
        <path class="st271" d="M574 2649.6c1.9 0 3.4 1.5 3.4 3.4s-1.5 3.4-3.4 3.4-3.4-1.5-3.4-3.4 1.5-3.4 3.4-3.4z"/>
        <path class="st288" d="M502.6 2675.5c3.1-5.7 9.1-8.8 13.5-8.8v8.8h-13.5z"/>
        <path class="st304" d="M529.6 2675.5c-3.1-5.7-9.1-8.8-13.5-8.8v8.8h13.5z"/>
        <path class="st288" d="M517.4 2673.3c.3 0 .5.2.5.5s-.2.5-.5.5-.5-.2-.5-.5.2-.5.5-.5zm5.5 0c.2 0 .3.1.3.3 0 .2-.1.3-.3.3s-.3-.1-.3-.3c-.1-.1.1-.3.3-.3zm-3.7.9c.2 0 .3.1.3.3 0 .2-.1.3-.3.3s-.3-.1-.3-.3c0-.1.2-.3.3-.3zm-1.2-2.6c.2 0 .3.1.3.3s-.1.3-.3.3-.3-.1-.3-.3.1-.3.3-.3z"/>
        <path class="st304" d="M513.3 2672.1c.4 0 .7.3.7.7 0 .4-.3.7-.7.7-.4 0-.7-.3-.7-.7 0-.4.3-.7.7-.7zm-2-2c.2 0 .5.2.5.5 0 .2-.2.5-.5.5-.2 0-.5-.2-.5-.5s.2-.5.5-.5zm3.2 3.7c.3 0 .5.2.5.5s-.2.5-.5.5-.5-.2-.5-.5.2-.5.5-.5zm-5.4 0c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4.2-.4.4-.4zm1.8-1.2c.3 0 .5.2.5.5s-.2.5-.5.5-.5-.2-.5-.5.2-.5.5-.5zm4-1.9c.2 0 .4.2.4.4s-.2.4-.4.4-.4-.2-.4-.4.2-.4.4-.4zm-2.2 3.3c.2 0 .3.1.3.3s-.1.3-.3.3c-.2 0-.3-.1-.3-.3s.2-.3.3-.3zm-6.6-1.2c.2 0 .3.1.3.3s-.1.3-.3.3-.3-.1-.3-.3.1-.3.3-.3z"/>
        <text transform="translate(484.162 2722.8)">
          <tspan x="0" y="0" class="st92 st90 st325">Campus</tspan><tspan x="-29.9" y="24.5" class="st92 st90 st325">Beautification</tspan>
        </text>
      </g>
      <g id="social-icon-2">
        <path class="st326" d="M801.8 2615h-89c-1.9 0-3.4 1.5-3.4 3.4v58.9c0 1.9 1.5 3.4 3.4 3.4h89c1.9 0 3.4-1.5 3.4-3.4v-58.9c.1-1.9-1.5-3.4-3.4-3.4zm1.1 62.3c0 .6-.5 1.1-1.1 1.1h-89c-.6 0-1.1-.5-1.1-1.1v-58.9c0-.6.5-1.1 1.1-1.1h89c.6 0 1.1.5 1.1 1.1v58.9z"/>
        <path class="st326" d="M721.8 2670.3h41.6c.9 0 1.6-.7 1.6-1.6v-41.6c0-.9-.7-1.6-1.6-1.6h-41.6c-.9 0-1.6.7-1.6 1.6v41.6c0 .8.7 1.6 1.6 1.6zm-.5-15h2.4c.5 3.3 1 4.9 1.9 4.9.9 0 1.4-1.5 1.9-4.9h.4v7h-6.6v-7zm10.4-14.6c.3 2.2.6 4.8.8 7h-4.2c.2-2.2.5-4.8.8-7h2.6zm-2.5-.2c.4-2.3.8-4 1.2-4 .5 0 .9 1.7 1.2 4h-2.4zm31.7.2c.3 2.2.6 4.8.8 7h-4.2c.2-2.2.5-4.8.8-7h2.6zm-2.6-.2c.4-2.3.8-4 1.2-4 .5 0 .9 1.7 1.2 4h-2.4zm3.4 7.5c.3 2.9.5 5.2.8 7h-5.2v-5.5c0-.5.1-1 .2-1.5h4.2zm-8.3 7c-.3-2.2-.6-4.9-.8-7h4.3c-.2 2.1-.5 4.8-.8 7h-2.7zm2.6.3c-.4 2.4-.8 4.3-1.3 4.3s-.9-1.9-1.3-4.3h2.6zm-27.8-5.7c.1-.5.1-1 .2-1.5h4.3c.3 2.9.5 5.2.8 7h-5.2v-5.5zm-.3 5.4h-.4c.1-.9.3-1.9.4-3v3zm5.3-7h2v7H734c-.3-2.2-.6-4.8-.8-7zm8.2-7.3c.3 2.2.6 4.8.8 7H738c.2-2.2.5-4.8.8-7h2.6zm-2.5-.2c.4-2.3.8-4 1.2-4 .5 0 .9 1.7 1.2 4h-2.4zm10.8.2v7h-2c.2-2.2.5-4.8.8-7h1.2zm-1.1-.2c.3-2.1.7-3.7 1.1-4v4h-1.1zm-1.4 7.2h-4.3c0-.4-.1-.9-.1-1.3v-5.8h5.3c-.4 1.9-.6 4.3-.9 7.1zm-3.5 7.3c-.3-2.2-.6-4.9-.8-7h4.3c-.2 2.2-.5 4.8-.8 7h-2.7zm2.6.3c-.4 2.4-.8 4.3-1.3 4.3s-.9-1.9-1.3-4.3h2.6zm-3.2-.3h-.4v-2.9c.2 1.1.3 2.1.4 2.9zm-.6-10.9c-.1-1.3-.3-2.4-.4-3.4h.4v3.4zm-.2 3.9c.1.6.1 1.2.2 1.7v5.3h-5.2c.3-1.8.5-4.1.8-7h4.2zm-5.7 7h-1.2v-7h2c-.2 2.2-.5 4.8-.8 7zm0 .3c-.3 2.2-.7 3.9-1.1 4.2v-4.2h1.1zm-1.4 0v4.2c-.4-.3-.8-2-1.1-4.2h1.1zm.2 4.8c.8-.2 1.3-1.7 1.7-4.9h5.3v7h-7v-2.1zm7.3-4.8h.4c.5 3.3 1 4.9 1.9 4.9.9 0 1.4-1.5 1.9-4.9h2.9v7h-7v-7zm4.2-.3c.3-1.8.5-4.1.8-7h2v7h-2.8zm3.1-7h2c.3 2.9.5 5.2.8 7H750v-7zm7 3.9v3.1h-.4c.2-.9.3-1.9.4-3.1zm.3-8v-3.2h.4c-.1 1-.3 2-.4 3.2zm-.3 2.4c0 .5-.1.9-.1 1.4h-4.3c-.3-2.9-.6-5.2-.8-7h5.3v5.6zm-5 1.4h-2v-7h1.1c.4 2.2.6 4.9.9 7zm-2-7.2v-4c.4.3.8 1.9 1.1 4H750zm-.3-4.6c-.8.1-1.3 1.6-1.7 4.6h-5.3v-7h7v2.4zm-7.2 4.6h-.5c-.5-3.2-1-4.6-1.8-4.6s-1.4 1.5-1.8 4.6h-2.9v-7h7v7zm-4.2.2c-.3 1.8-.5 4.1-.8 7h-2v-7h2.8zm-3.1 7h-2c-.3-2.9-.6-5.2-.8-7h2.9v7zm-7-3.7v-3.2h.4c-.2.9-.3 1.9-.4 3.2zm-.3 2.4c0 .4-.1.9-.1 1.4h-4.3c-.3-2.9-.6-5.2-.8-7h5.3v5.6zm-.2 1.6c-.2 2.1-.5 4.8-.8 7h-2.6c-.3-2.2-.6-4.9-.8-7h4.2zm-.8 7.3c-.4 2.4-.8 4.3-1.3 4.3s-.9-1.9-1.3-4.3h2.6zm1.3 0h5.3c.5 3.2 1 4.7 1.8 4.9v2.2h-7v-7.1zm7 7.3v6.6h-7v-6.6h7zm.2 0h7v6.6h-7v-6.6zm7.3 0h7v6.6h-7v-6.6zm7.3 0h7v6.6h-7v-6.6zm0-.3v-7h2.8c.5 3.3 1 4.9 1.9 4.9.9 0 1.4-1.5 1.9-4.9h.4v7h-7zm7.3-7h5.3c.4 2.6.8 4.1 1.4 4.6v2.4h-6.6v-7zm6.6 3.5c-.3-.8-.5-2-.8-3.6h.8v3.6zm-.8-3.8c-.3-2.2-.6-4.9-.8-7h1.6v7h-.8zm.8-7.3h-1.6c-.3-2.9-.6-5.2-.8-7h2.5v7zm-2.5-7.2c-.5-3.2-1-4.6-1.8-4.6s-1.4 1.5-1.8 4.6h-.4v-7h6.6v7h-2.6zm-4.4 0h-5.3c-.5-3-.9-4.4-1.7-4.6v-2.4h7v7zm-7-7.3v-6.6h7v6.6h-7zm-.3 0h-7v-6.6h7v6.6zm-7.2 0h-7v-6.6h7v6.6zm-7.3 0h-7v-6.6h7v6.6zm0 .2v7h-2.9c-.5-3.2-1-4.6-1.8-4.6s-1.4 1.5-1.8 4.6h-.5v-7h7zm-7.3 7.1h-5.3c-.4-2.4-.8-3.9-1.3-4.4v-2.6h6.6v7zm-5.9 0h-.7v-3.3c.2.7.5 1.9.7 3.3zm-.7.2h.7c.3 2.2.6 4.8.8 7h-1.6v-7zm1.6 7.3c.3 2.9.5 5.2.8 7h-2.4v-7h1.6zm-1.6 20.7v-6.1h6.6v6.6h-6.1c-.3 0-.5-.2-.5-.5zm42.1.5h-6.1v-6.6h6.6v6.1c0 .3-.2.5-.5.5zm.5-42.1v6.1h-6.6v-6.6h6.1c.3 0 .5.2.5.5zm-42.1-.5h6.1v6.6h-6.6v-6.1c0-.3.2-.5.5-.5z"/>
        <circle class="st326" cx="775.7" cy="2631.1" r="2"/>
        <circle class="st326" cx="791.9" cy="2631.1" r="2"/>
        <path class="st326" d="M777.1 2670.3c.9 0 1.8-.2 2.6-.6.4-.2.7-.4 1-.6.3-.2.6-.5.8-.8.8-1 1.3-2.2 1.3-3.6 0-3.2-2.6-5.7-5.7-5.7-.9 0-1.8.2-2.6.6-.4.2-.7.4-1 .6-1.3 1-2.1 2.6-2.1 4.4 0 3.1 2.6 5.7 5.7 5.7zm0-10c2.4 0 4.3 1.9 4.3 4.3 0 .9-.3 1.8-.8 2.4l-5.2-6.4c.6-.2 1.1-.3 1.7-.3zm-3.5 1.8l5.2 6.4c-.5.2-1.1.3-1.7.3-2.4 0-4.3-1.9-4.3-4.3 0-.9.3-1.7.8-2.4z"/>
        <path class="st326" d="M713.2 2677h88.3v-58.2h-88.3v58.2zm87.1-11.1c-.4 1.9-1.4 3.5-3 4.6-1.2.8-2.6 1.2-4 1.2-2.4 0-4.6-1.2-5.9-3.1-1.1-1.6-1.5-3.5-1.1-5.3.4-1.9 1.4-3.5 3-4.6 1.2-.8 2.6-1.2 4-1.2 2.4 0 4.6 1.2 5.9 3.1 1.1 1.5 1.4 3.4 1.1 5.3zm-26.7-17.9v-5.4h2.1v5.4h.6v-5.4h2.1v9h.6v-9h1v11.8h-8c-.3 0-.6-.3-.6-.6v-10.6c0-.3.3-.6.6-.6h1.2v5.4h.4zm7.4 0h.5v-5.4h2.1v5.4h.6v-5.4h2.1v9h.6v-9h2.1v5.4h.6v-5.4h2.1v5.4h.6v-5.4h2.1v9h.6v-9h2.1v5.4h.6v-5.4h1.2c.3 0 .6.3.6.6v10.6c0 .3-.3.6-.6.6H781v-6.4zm12.3-22c3.6 0 6.5 2.9 6.5 6.5s-2.9 6.5-6.5 6.5-6.5-2.9-6.5-6.5 2.9-6.5 6.5-6.5zm-16.2 0c3.6 0 6.5 2.9 6.5 6.5s-2.9 6.5-6.5 6.5-6.5-2.9-6.5-6.5 2.9-6.5 6.5-6.5zm0 31.4c3.9 0 7.1 3.2 7.1 7.1 0 3.9-3.2 7.1-7.1 7.1-3.9 0-7.1-3.2-7.1-7.1 0-3.9 3.2-7.1 7.1-7.1zm-58.3-30.3c0-1.7 1.3-3 3-3h41.6c1.7 0 3 1.3 3 3v41.6c0 1.7-1.3 3-3 3h-41.6c-1.7 0-3-1.3-3-3v-41.6z"/>
        <path class="st326" d="M793.3 2658.8c-1.1 0-2.2.3-3.2 1-2.6 1.8-3.3 5.3-1.5 7.9 1.1 1.6 2.9 2.5 4.7 2.5 1.1 0 2.2-.3 3.2-1 2.6-1.8 3.3-5.3 1.5-7.9-1.1-1.6-2.9-2.5-4.7-2.5zm-3.6 8.1c-.6-.9-.9-2.1-.7-3.2.2-1.1.9-2.1 1.8-2.7.7-.5 1.5-.7 2.4-.7h.1l-2.4 7.8c-.4-.3-.8-.7-1.2-1.2zm7.8-1.5c-.2 1.1-.9 2.1-1.8 2.7-.7.5-1.5.7-2.4.7h-.1l2.4-7.8c.5.3.9.7 1.2 1.2.7.9.9 2 .7 3.2z"/>
        <path class="st327" d="M729.6 2647.6v.8c0 .5-.1 1.3-.2 2.3-.1 1-.3 2.2-.7 3.5-.4 1.3-.9 2.8-1.9 4.2-.5.7-1 1.4-1.7 2.1-.7.6-1.6 1.2-2.5 1.4-.3.1-.5.1-.8.1h-.8c-.2 0-.5 0-.7-.1-.3-.1-.5-.1-.8-.2-1-.4-1.8-1.1-2.5-1.9-.7-.8-1.3-1.7-1.7-2.7l-.6-1.5c-.2-.5-.4-1-.5-1.6-.5-2.1-.8-4.3-.8-6.5s.3-4.4.8-6.5c.1-.5.3-1 .5-1.6l.6-1.5c.4-1 1-1.9 1.7-2.7.7-.8 1.5-1.5 2.5-1.9.2-.1.5-.2.8-.2.3-.1.5-.1.8-.1h.8c.2 0 .5.1.8.1.1 0 .3.1.4.1l.3.2c.2.1.5.2.7.3.2.1.4.3.6.4.2.2.4.3.5.5.7.6 1.3 1.3 1.7 2.1.9 1.4 1.5 2.9 1.9 4.2.4 1.3.6 2.5.7 3.5.1 1 .2 1.7.2 2.3-.1.6-.1.9-.1.9zm-1.3 0v-.8c0-.5-.1-1.2-.1-2.2-.1-.5-.1-1-.2-1.5-.1-.3-.1-.6-.2-.9-.1-.3-.1-.6-.2-.9-.3-1.2-.8-2.6-1.6-4-.4-.7-.9-1.3-1.5-1.9-.6-.6-1.3-1.1-2.1-1.3-.2-.1-.4-.1-.6-.2h-.7c-.2 0-.4 0-.7.1-.2.1-.4.1-.7.2-.9.3-1.7.9-2.3 1.6-.4.3-.6.8-1 1.2-.3.4-.6.9-.8 1.3-.5.9-.9 1.9-1.2 2.9-.6 2.1-.9 4.2-.9 6.4s.3 4.4.9 6.4c.3 1 .7 2 1.2 2.9.2.5.5.9.8 1.3.3.4.6.8 1 1.2.7.7 1.5 1.3 2.3 1.6.2.1.4.1.6.2.2 0 .5 0 .7.1h.1s-.1 0 0 0h.5c.2 0 .4-.1.6-.1.8-.3 1.5-.7 2.1-1.3.6-.6 1.1-1.2 1.5-1.9.8-1.4 1.3-2.7 1.6-4 .1-.3.2-.6.2-.9.1-.3.1-.6.2-.9.1-.5.2-1.1.2-1.5.1-.9.1-1.6.1-2.2.2-.6.2-.9.2-.9z"/>
        <path class="st327" d="M725.4 2640.3s.2.1.7.4c.4.3 1.1.7 1.9 1.3.8.6 1.7 1.3 2.7 2.4.9 1 1.9 2.2 2.7 3.7.4.8.7 1.6.9 2.5.2.9.2 1.9 0 2.9-.1.2-.1.5-.3.7l-.2.4-.1.2v.1l-.1.1c-.2.2-.3.4-.5.6l-.6.6c-.8.7-1.9 1-2.9 1.2-1 .2-2.1.2-3.2.1-.5 0-1.1-.1-1.6-.2s-1.1-.2-1.6-.4c-2.1-.6-4.1-1.4-6.1-2.5-1.9-1.1-3.7-2.4-5.2-4-.4-.4-.7-.8-1.1-1.2-.3-.4-.7-.8-1-1.3-.6-.9-1.1-1.8-1.5-2.8-.3-1-.5-2.1-.4-3.1 0-.3.1-.5.2-.8.1-.3.2-.5.3-.7v-.2l.1-.2.2-.3c.1-.2.3-.4.5-.6l.3-.3.3-.2c.2-.1.4-.3.6-.4.2-.1.4-.2.7-.3.2-.1.4-.2.7-.2.9-.3 1.8-.4 2.7-.5 1.7-.1 3.3.2 4.6.5 1.3.3 2.5.8 3.4 1.1.9.4 1.6.7 2.1 1l.8.4zm-.7 1.2s-.3-.1-.7-.4c-.4-.3-1.1-.6-1.9-1-.4-.2-.9-.4-1.4-.6-.3-.1-.5-.2-.8-.3l-.9-.3c-1.2-.3-2.7-.6-4.3-.6-.8 0-1.6.1-2.4.3-.8.2-1.6.6-2.2 1.1-.1.1-.3.3-.4.5l-.2.3-.1.1v.1l-.3.6c-.1.2-.1.4-.2.7-.2.9-.1 1.9.2 2.8.1.5.3.9.5 1.4.2.5.5.9.8 1.3.5.9 1.2 1.7 2 2.5 1.5 1.6 3.2 2.9 5.1 4 1.9 1.1 3.9 1.9 6 2.4 1 .2 2.1.4 3.1.4h1.5c.5-.1 1-.1 1.5-.2 1-.2 1.9-.6 2.6-1.2l.5-.5c.1-.2.3-.4.4-.6l.1-.1.1-.2.1-.3c.1-.2.1-.4.2-.6.2-.8.1-1.7-.1-2.5s-.5-1.6-.9-2.2c-.8-1.4-1.7-2.5-2.6-3.4-.2-.2-.5-.4-.7-.7-.2-.2-.4-.4-.7-.6-.4-.4-.8-.7-1.2-1-.8-.5-1.3-.9-1.8-1.2-.6.1-.8 0-.9 0z"/>
        <path class="st327" d="M725.4 2654.9s-.2.1-.7.4c-.4.2-1.2.6-2.1 1-.9.4-2 .8-3.4 1.1-1.3.3-2.9.6-4.6.5-.9 0-1.8-.2-2.7-.5-.9-.3-1.8-.8-2.5-1.5-.2-.2-.4-.4-.5-.6l-.2-.3-.1-.2v-.2c-.1-.2-.2-.4-.3-.7-.1-.3-.1-.5-.2-.8-.2-1.1 0-2.1.4-3.1.3-1 .9-2 1.5-2.8.3-.5.6-.9 1-1.3s.7-.8 1.1-1.2c1.5-1.5 3.3-2.9 5.2-4 1.9-1.1 4-2 6-2.5.5-.1 1.1-.2 1.6-.4.5-.1 1.1-.2 1.6-.2 1.1-.1 2.1-.1 3.2.1 1 .2 2.1.6 2.9 1.2.2.2.4.4.6.5.2.2.3.4.5.6l.1.1v.1l.1.2.2.3c.1.2.2.5.3.7 0 .1.1.3.1.4v.4c0 .3.1.5 0 .7v.7c0 .2-.1.5-.1.7-.2.9-.5 1.8-.9 2.5-.8 1.5-1.8 2.7-2.7 3.7-.9 1-1.9 1.8-2.7 2.4-.8.6-1.4 1-1.9 1.3-.5.6-.8.7-.8.7zm-.6-1.1s.2-.1.7-.4c.4-.2 1-.7 1.8-1.2.4-.3.8-.6 1.2-1 .2-.2.4-.4.7-.6l.7-.7c.9-.9 1.9-2 2.6-3.4.4-.7.7-1.4.9-2.2.2-.8.3-1.7.1-2.5-.1-.2-.1-.4-.2-.6l-.1-.3-.1-.2v-.1c-.1-.2-.2-.4-.4-.5l-.5-.5c-.7-.6-1.6-1-2.6-1.2-.5-.1-1-.2-1.5-.2s-1-.1-1.5 0c-1 0-2.1.2-3.1.4-2.1.5-4.1 1.3-6 2.4-1.9 1.1-3.6 2.4-5.1 4-.7.8-1.4 1.6-2 2.5-.3.4-.5.9-.8 1.3-.2.5-.4.9-.5 1.4-.3.9-.4 1.9-.2 2.8.1.2.1.4.2.6l.3.6v.1s0-.1 0 0l.1.1.2.3c.1.2.3.3.4.5.6.6 1.4 1 2.2 1.2.8.2 1.6.3 2.4.3 1.6 0 3-.3 4.3-.6l.9-.3c.3-.1.6-.2.8-.3.5-.2 1-.4 1.4-.6.8-.4 1.5-.7 1.9-1 .5 0 .8-.2.8-.1z"/>
        <circle class="st328" cx="721.2" cy="2647.6" r="3.4"/>
        <circle class="st329" cx="722.1" cy="2646.7" r="2"/>
        <circle class="st330" cx="715.5" cy="2637.9" r="2.1"/>
        <circle class="st331" cx="716" cy="2637.3" r="1.3"/>
        <circle class="st330" cx="715.5" cy="2657.4" r="2.1"/>
        <circle class="st331" cx="716" cy="2656.8" r="1.3"/>
        <circle class="st330" cx="732.3" cy="2647.6" r="2.1"/>
        <circle class="st331" cx="732.9" cy="2647.1" r="1.3"/>
        <path class="st11" d="M740.6 2604.8v18.6c0 1.6-1.3 3-3 3-1.6 0-3-1.3-3-3v-18.6h6z"/>
        <path class="st328" d="M739.8 2611.1v12.3c0 1.2-1 2.1-2.1 2.1-1.2 0-2.1-1-2.1-2.1v-12.3h4.2z"/>
        <path class="st332" d="M734.7 2605.7h6c.5 0 .9-.4.9-.9s-.4-.9-.9-.9h-6c-.5 0-.9.4-.9.9s.4.9.9.9zm0 1.2h2v.4h-2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.7h2v.4h-2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2z"/>
        <path class="st11" d="M730.8 2604.8v18.6c0 1.6-1.3 3-3 3-1.6 0-3-1.3-3-3v-18.6h6z"/>
        <path class="st327" d="M730 2615.2v8.2c0 1.2-1 2.1-2.1 2.1-1.2 0-2.1-1-2.1-2.1v-8.2h4.2z"/>
        <path class="st332" d="M724.9 2605.7h5.9c.5 0 .9-.4.9-.9s-.4-.9-.9-.9h-5.9c-.5 0-.9.4-.9.9s.4.9.9.9zm0 1.2h2v.4h-2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.7h2v.4h-2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2zm0 1.6h1.2v.4h-1.2z"/>
        <path class="st11" d="M721 2604.8v18.6c0 1.6-1.3 3-3 3-1.6 0-3-1.3-3-3v-18.6h6z"/>
        <path class="st330" d="M720.2 2613.2v10.2c0 1.2-1 2.1-2.1 2.1s-2.1-1-2.1-2.1v-10.2h4.2z"/>
        <path class="st332" d="M715 2605.7h6c.5 0 .9-.4.9-.9s-.4-.9-.9-.9h-6c-.5 0-.9.4-.9.9s.4.9.9.9zm0 1.2h2v.4h-2zm0 1.6h1.2v.4H715zm0 1.6h1.2v.4H715zm0 1.6h1.2v.4H715zm0 1.6h1.2v.4H715zm0 1.7h2v.4h-2zm0 1.6h1.2v.4H715zm0 1.6h1.2v.4H715zm0 1.6h1.2v.4H715zm0 1.6h1.2v.4H715z"/>
        <path class="st333" d="M710.7 2615.5H745c.2 0 .4-.2.4-.4s-.2-.4-.4-.4h-34.4c-.2 0-.4.2-.4.4 0 .3.2.4.5.4z"/>
        <path class="st333" d="M713.4 2627.6c.2 0 .4-.2.4-.4v-12.1c0-.2-.2-.4-.4-.4s-.4.2-.4.4v12.1c0 .2.2.4.4.4zm28.9 0c.2 0 .4-.2.4-.4v-12.1c0-.2-.2-.4-.4-.4s-.4.2-.4.4v12.1c0 .2.2.4.4.4z"/>
        <path class="st334" d="M710.7 2628H745c.5 0 .8-.4.8-.8 0-.5-.4-.8-.8-.8h-34.4c-.5 0-.8.4-.8.8 0 .5.4.8.9.8z"/>
        <path class="st11" d="M775.4 2600.6h9.6v4.3h-9.6z"/>
        <path class="st335" d="M775.4 2620.3c0 2.2-1.8 4-4 4v9.6c7.5 0 13.6-6.1 13.6-13.6v-15.4h-9.6v15.4z"/>
        <path class="st11" d="M757.7 2600.6h9.6v4.3h-9.6z"/>
        <path class="st327" d="M767.3 2620.3v-15.4h-9.6v15.4c0 7.5 6.1 13.6 13.6 13.6v-9.6c-2.2.1-4-1.7-4-4z"/>
        <path class="st330" d="M764.9 2588.2c-1.5.3-2.9.7-4.3 1.2.1-.4.3-.9.4-1.3.2-.6.3-1.3.5-1.9.2-.6.3-1.3.4-2-.4.5-.8 1-1.2 1.6-.4.5-.8 1.1-1.1 1.6-.7 1.1-1.4 2.2-2 3.4l-1.2 2.2 2.7-.5c1.1-.2 2.1-.4 3.1-.7l-.9 1.5c-.5.8-.9 1.6-1.3 2.4-.2.4-.4.8-.6 1.3-.2.4-.4.9-.6 1.3.4-.3.7-.6 1.1-.9.4-.3.7-.6 1-.9.7-.6 1.3-1.3 2-2 1.3-1.3 2.5-2.7 3.6-4.2l2.5-3.1-4.1 1zm17.6 0c-1.5.3-2.9.7-4.3 1.2.1-.4.3-.9.4-1.3.2-.6.3-1.3.5-1.9.2-.6.3-1.3.4-2-.4.5-.8 1-1.2 1.6-.4.5-.8 1.1-1.1 1.6-.7 1.1-1.4 2.2-2 3.4l-1.2 2.2 2.7-.5c1.1-.2 2.1-.4 3.1-.7l-.9 1.5c-.5.8-.9 1.6-1.3 2.4-.2.4-.4.8-.6 1.3-.2.4-.4.9-.6 1.3.4-.3.7-.6 1.1-.9.4-.3.7-.6 1-.9.7-.6 1.3-1.3 2-2 1.3-1.3 2.5-2.7 3.6-4.2l2.5-3.1-4.1 1z"/>
        <path class="st11" d="M802.725 2624.83l4.808-4.808 3.394 3.394-4.808 4.81z"/>
        <path class="st334" d="M783.913 2644.33l3.96-3.96 2.828 2.83-3.95 3.96z"/>
        <path class="st11" d="M786.77 2639.105l15.908-15.912 5.233 5.23-15.9 15.913z"/>
        <path class="st11" d="M791.2 2657.5c-3.5 0-6.8-1.4-9.2-3.8l2.6-2.6c1.8 1.8 4.2 2.8 6.7 2.8s4.9-1 6.7-2.8c3.7-3.7 3.7-9.7 0-13.4l2.6-2.6c5.1 5.1 5.1 13.4 0 18.5-2.6 2.5-5.9 3.9-9.4 3.9z"/>
        <path class="st336" d="M777.7 2651h12.4v2.8h-12.4zm13.9 14.7c-2.2 0-4-1.8-4-4v-3.2c0-2.2 1.8-4 4-4s4 1.8 4 4v3.2c.1 2.2-1.8 4-4 4z"/>
        <path class="st11" d="M798.9 2664v-2c0-.5-.4-1-1-1h-13.1c-.5 0-1 .4-1 1v2h15.1z"/>
        <path class="st336" d="M800.9 2667v-2c0-.5-.4-1-1-1h-17.1c-.5 0-1 .4-1 1v2h19.1z"/>
        <circle class="st334" cx="791.6" cy="2658.5" r="1.5"/>
        <path class="st336" d="M792 2645.6c-.4 0-.7-.1-1-.4l-5.2-5.2c-.6-.6-.6-1.4 0-2 .6-.6 1.4-.6 2 0l5.2 5.2c.6.6.6 1.4 0 2-.2.3-.6.4-1 .4zm16-15.9c-.4 0-.7-.1-1-.4l-5.2-5.2c-.6-.6-.6-1.4 0-2 .6-.6 1.4-.6 2 0l5.2 5.2c.6.6.6 1.4 0 2-.3.3-.7.4-1 .4zm2.9-5.2c-.2 0-.4-.1-.6-.2l-3.5-3.5c-.3-.3-.3-.8 0-1.1.3-.3.8-.3 1.1 0l3.5 3.5c.3.3.3.8 0 1.1-.1.1-.3.2-.5.2z"/>
        <path class="st11" d="M783.3 2679l-17.8-26.2c-.7-1-1.2-2.7-1.2-3.9v-21.8h-13.9v21.8c0 1.2-.5 2.9-1.2 3.9l-17.8 26.2c-.7 1-.2 1.8.9 1.8h50.1c1.1 0 1.6-.8.9-1.8z"/>
        <path class="st328" d="M745.7 2661.7l-11.5 16.9h46.3l-11.5-16.9z"/>
        <path class="st332" d="M764.3 2629.3h-13.9c-1.2 0-2.1-1-2.1-2.1s1-2.1 2.1-2.1h13.9c1.2 0 2.1 1 2.1 2.1s-.9 2.1-2.1 2.1z"/>
        <circle class="st337" cx="748.3" cy="2669" r="3.3"/>
        <circle class="st337" cx="759.1" cy="2665.6" r="1.7"/>
        <circle class="st337" cx="765.7" cy="2672.3" r="4"/>
        <circle class="st337" cx="755.5" cy="2674.1" r=".9"/>
        <circle class="st337" cx="761.9" cy="2657.7" r="2.7"/>
        <circle class="st337" cx="753.9" cy="2654.9" r="1.8"/>
        <circle class="st337" cx="758.5" cy="2648.4" r="1.2"/>
        <text transform="translate(716.06 2722.8)">
          <tspan x="0" y="0" class="st92 st90 st325">Research</tspan><tspan x="-29.8" y="24.5" class="st92 st90 st325">&amp; Development</tspan>
        </text>
      </g>
      <g id="social-icon-1">
        <path class="st338" d="M289 2659.3c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2658.9c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2654.9v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1V2651c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2654.9c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.9 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2655.1" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2654.5" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2652c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2653.6c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2653.2c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2649.2v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2 0 .5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7V2645h-.7zm1.3 0v12.4h.7V2645h-.7zm1.5 0v12.4h.7V2645h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2V2646c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2649.2c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2649.4" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2648.8" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2646.3c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2647.9c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2647.5c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2643.5v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2 0 .5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1V2640c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2643.5c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2643.7" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2643.1" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2640.6c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2642.2c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2641.8c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2637.8v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1V2634c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2637.8c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2638" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2637.4" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2634.9c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2636.5c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2636.1c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2632.1v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.1-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1V2628c-.2 0-.5.1-.7.1zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2632.1c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2632.3" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2631.7" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2629.2c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2630.8c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2630.4c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2626.4v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2V2623c-.2.1-.5.1-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2626.4c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2626.6" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2626" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2623.5c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2625.1c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2624.7c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2620.7v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.1-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.1-.7.2zm1.5-.4v11.1c.2 0 .5.1.7.1V2617c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2620.7c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2620.9" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2620.3" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2617.8c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2619.4c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2619c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2615v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.1-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.1-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1V2611c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.1v11.8c.2 0 .5-.1.7-.1v-11.6c-.3 0-.5 0-.7-.1zm1.4.3v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2615c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2615.2" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2614.6" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2612.1c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2613.7c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2613.2c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2609.3v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.1-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.1-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7V2605c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.1v11.8c.2 0 .5-.1.7-.1v-11.6c-.3 0-.5 0-.7-.1zm1.4.3v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M289 2609.3c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="276.3" cy="2609.5" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2608.9" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2606.4c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M289 2608c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M289 2607.5c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M263.7 2603.6v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.5.3.7.4v-8.7c-.3.1-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.1-.7.2zm1.5-.4v11.1c.2 0 .5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5-.1-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.6v12.3h.7l-.1-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.1v11.8c.2 0 .5-.1.7-.1v-11.6c-.3 0-.5 0-.7-.1zm1.4.3v11.4c.2 0 .5-.1.7-.1V2600c-.2 0-.4-.1-.7-.1zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <ellipse class="st340" cx="276.3" cy="2603.6" rx="12.6" ry="4.2"/>
        <ellipse class="st341" cx="276.3" cy="2603.8" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="276.3" cy="2603.2" rx="10.4" ry="3.1"/>
        <path class="st339" d="M276.3 2600.7c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M264.6 2655.7c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M264.6 2655.3c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M239.3 2651.3v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.4.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.2-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.1v12.2h.7v-12.3c-.2 0-.5 0-.7.1zm1.3-.1v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.7v12.3h.7v-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M264.6 2651.3c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.9 12.6 4.2z"/>
        <ellipse class="st341" cx="251.9" cy="2651.5" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="251.9" cy="2650.9" rx="10.4" ry="3.1"/>
        <path class="st339" d="M251.9 2648.4c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.5 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M264.6 2650c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M264.6 2649.6c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M239.3 2645.6v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.4.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.2-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2 0 .5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.1v12.2h.7v-12.3c-.2 0-.5 0-.7.1zm1.3-.1v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.7v12.3h.7v-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1V2642c-.2 0-.4-.1-.7-.1zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M264.6 2645.6c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.9 12.6 4.2z"/>
        <ellipse class="st341" cx="251.9" cy="2645.8" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="251.9" cy="2645.2" rx="10.4" ry="3.1"/>
        <path class="st339" d="M251.9 2642.7c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.5 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M264.6 2644.3c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M264.6 2643.9c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M239.3 2639.9v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.4.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.2-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2 0 .5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1V2636c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.7v12.3h.7v-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M264.6 2639.9c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.9 12.6 4.2z"/>
        <ellipse class="st341" cx="251.9" cy="2640.1" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="251.9" cy="2639.5" rx="10.4" ry="3.1"/>
        <path class="st339" d="M251.9 2637c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.5 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M264.6 2638.6c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M264.6 2638.2c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M239.3 2634.2v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.4.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7V2630h-.7zm1.3 0v12.4h.7V2630h-.7zm1.5 0v12.4h.7V2630h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.7v12.3h.7V2630c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2V2631c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M264.6 2634.2c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.9 12.6 4.2z"/>
        <ellipse class="st341" cx="251.9" cy="2634.4" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="251.9" cy="2633.8" rx="10.4" ry="3.1"/>
        <path class="st339" d="M251.9 2631.3c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M264.6 2632.9c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M264.6 2632.5c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M239.3 2628.5v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.4.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.7v12.3h.7v-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1V2625c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M264.6 2628.5c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="251.9" cy="2628.7" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="251.9" cy="2628.1" rx="10.4" ry="3.1"/>
        <path class="st339" d="M251.9 2625.6c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M264.6 2627.2c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M264.6 2626.8c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M239.3 2622.8v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.5-2v7.9c.2.1.4.3.7.4v-8.7c-.3.2-.5.3-.7.4zm1.3-.7v9.3c.2.1.5.2.7.3v-9.8c-.2.1-.5.1-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.2.1-.5.2-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0 0 0 0 0zm-.1 0h-.7v12.3h.7v-12.3c.1 0 0 0 0 0zm.9.1v12.2c.2 0 .5 0 .7-.1v-12c-.3-.1-.5-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1V2619c-.3-.1-.5-.1-.7-.1zm1.4.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.2-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.2 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.2-.1-.5-.3-.7-.4zm2.2 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.4-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M264.6 2622.8c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 6.9 0 12.6 1.8 12.6 4.2z"/>
        <ellipse class="st341" cx="251.9" cy="2623" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="251.9" cy="2622.4" rx="10.4" ry="3.1"/>
        <path class="st339" d="M251.9 2619.9c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.6 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M271 2665.8c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M271 2665.4c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M245.8 2661.4v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.4-2v7.9c.2.1.4.3.7.4v-8.7c-.2.2-.4.3-.7.4zm1.4-.7v9.3c.2.1.5.2.7.3v-9.8c-.3.1-.5.2-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2V2658c-.3.1-.5.2-.7.2zm1.5-.4v11.1c.2.1.5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.1v12.2h.7v-12.3c-.2 0-.5 0-.7.1zm1.3-.1v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0-.1 0 0 0zm-.1 0h-.7v12.3h.7v-12.3zm.8.1v12.2c.2 0 .5 0 .7-.1v-12c-.2-.1-.4-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.2-.1-.4-.1-.7-.1zm1.5.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.3-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.3 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.3-.1-.5-.3-.7-.4zm2.1 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.5-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M271 2661.4c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2z"/>
        <ellipse class="st341" cx="258.4" cy="2661.6" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="258.4" cy="2661" rx="10.4" ry="3.1"/>
        <path class="st339" d="M258.4 2658.5c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.5 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M271 2660.1c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M271 2659.7c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M245.8 2655.7v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.4-2v7.9c.2.1.4.3.7.4v-8.7c-.2.2-.4.3-.7.4zm1.4-.7v9.3c.2.1.5.2.7.3v-9.8c-.3.1-.5.2-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.3.1-.5.2-.7.2zm1.5-.4v11.1c.2 0 .5.1.7.1V2652c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1v-12.1c-.2-.1-.5 0-.7 0zm1.5-.1v12.2h.7v-12.3c-.2 0-.5 0-.7.1zm1.3-.1v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0-.1 0 0 0zm-.1 0h-.7v12.3h.7v-12.3zm.8.1v12.2c.2 0 .5 0 .7-.1v-12c-.2-.1-.4-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.2-.1-.4-.1-.7-.1zm1.5.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.3-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.3 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.3-.1-.5-.3-.7-.4zm2.1 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.5-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M271 2655.7c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2z"/>
        <ellipse class="st341" cx="258.4" cy="2655.9" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="258.4" cy="2655.3" rx="10.4" ry="3.1"/>
        <path class="st339" d="M258.4 2652.8c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.5 5-2.8 10.4-2.8z"/>
        <path class="st338" d="M271 2654.4c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st339" d="M271 2654c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2v-4c0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2v4z"/>
        <path class="st338" d="M245.8 2650v4c0 .5.2.9.7 1.3v-6.7c-.5.5-.7.9-.7 1.4zm1.4-2v7.9c.2.1.4.3.7.4v-8.7c-.2.2-.4.3-.7.4zm1.4-.7v9.3c.2.1.5.2.7.3v-9.8c-.3.1-.5.2-.7.2zm1.5-.5v10.3c.2.1.5.1.7.2v-10.7c-.3.1-.5.2-.7.2zm1.5-.4v11.1c.2 0 .5.1.7.1v-11.3c-.3 0-.5.1-.7.1zm1.5-.2v11.6c.2 0 .5.1.7.1v-11.8c-.3 0-.5 0-.7.1zm1.3-.2v12c.2 0 .5.1.7.1V2646c-.2-.1-.5 0-.7 0zm1.5-.2v12.2h.7v-12.3c-.2.1-.5.1-.7.1zm1.3 0v12.4h.7v-12.4h-.7zm1.5 0v12.4h.7v-12.4h-.7zm2.1 0c-.1 0-.1 0 0 0zm-.1 0h-.7v12.3h.7v-12.3zm.8.1v12.2c.2 0 .5 0 .7-.1v-12c-.2-.1-.4-.1-.7-.1zm1.5.2v11.8c.2 0 .5-.1.7-.1v-11.6c-.2-.1-.4-.1-.7-.1zm1.5.2v11.4c.2 0 .5-.1.7-.1v-11.1c-.2-.1-.4-.2-.7-.2zm1.4.3v10.8c.2-.1.5-.1.7-.2v-10.4c-.3-.1-.5-.2-.7-.2zm1.5.4v9.9c.2-.1.5-.2.7-.3v-9.4c-.3 0-.5-.1-.7-.2zm1.5.6v8.7c.3-.1.5-.3.7-.4v-7.9c-.3-.1-.5-.3-.7-.4zm2.1 6.4v-4c0-.5-.2-1-.7-1.4v6.7c.5-.4.7-.9.7-1.3z"/>
        <path class="st340" d="M271 2650c0 2.3-5.7 4.2-12.6 4.2-7 0-12.6-1.9-12.6-4.2 0-2.3 5.7-4.2 12.6-4.2 7 0 12.6 1.9 12.6 4.2z"/>
        <ellipse class="st341" cx="258.4" cy="2650.2" rx="10.4" ry="3.1"/>
        <ellipse class="st342" cx="258.4" cy="2649.6" rx="10.4" ry="3.1"/>
        <path class="st339" d="M258.4 2647.1c5.4 0 9.9 1.2 10.4 2.8v-.3c0-1.7-4.7-3.1-10.4-3.1-5.8 0-10.4 1.4-10.4 3.1v.3c.5-1.5 5-2.8 10.4-2.8zm28 14h4.9v7.3h-4.9z"/>
        <path class="st339" d="M351.8 2664.1l-37 14-26.6-10.1 37-14z"/>
        <path class="st340" d="M314.8 2678.1l37-14v2.7l-37 14-26.8-10.3.2-2.5z"/>
        <path class="st343" d="M350.9 2663.6l-36 13.6v-19.9h36z"/>
        <path class="st11" d="M288 2662.1c.1 0 .2 0 .3.1l26.5 8v7.1l-26.6-10.1c-.7-.8-1.2-2-1.2-3.3.1-1 .5-1.8 1-1.8z"/>
        <path class="st339" d="M325.2 2645.7l26.6 10.1-37 14-.8-.3-1 .4-26.7-10.1 37.9-14.4z"/>
        <path class="st340" d="M314.8 2669.8l37-14v2.7l-37 14-26.6-10.1.3-2.5z"/>
        <path class="st340" d="M287.4 2659.7c.4 0 .8.1 1.2.2l24.6 9.3v2.7l-25.5-9.7c-.1 0-.2-.1-.3-.1-.5 0-.9.8-.9 1.8 0 1.9 1.1 3.6 2.1 4l24.6 9.4v2.7l-25.5-9.8c-1.1-.4-2-1.3-2.7-2.5-.7-1.2-1-2.5-1-3.8 0-1.2.3-2.2.8-3 .7-.7 1.6-1.2 2.6-1.2z"/>
        <path class="st344" d="M286.4 2650.2h4.9v7.3h-4.9z"/>
        <path class="st344" d="M351.8 2653.1l-37 14-26.6-10.1 37-13.9z"/>
        <path class="st345" d="M314.8 2667.1l37-14v2.7l-37 14-26.8-10.3.2-2.5z"/>
        <path class="st343" d="M350.9 2652.7l-36 13.6v-20h36z"/>
        <path class="st11" d="M288 2651.1c.1 0 .2 0 .3.1l26.5 8v7.1l-26.6-10.1c-.7-.8-1.2-2-1.2-3.3.1-1 .5-1.8 1-1.8z"/>
        <path class="st344" d="M325.2 2634.8l26.6 10-37 14-.8-.3-1 .4-26.7-10 37.9-14.5z"/>
        <path class="st345" d="M314.8 2658.8l37-14v2.7l-37 14-26.6-10.1.3-2.5z"/>
        <path class="st345" d="M287.4 2648.7c.4 0 .8.1 1.2.2l24.6 9.3v2.7l-25.5-9.7c-.1 0-.2-.1-.3-.1-.5 0-.9.8-.9 1.8 0 1.9 1.1 3.6 2.1 4l24.6 9.4v2.7l-25.5-9.8c-1.1-.4-2-1.3-2.7-2.5-.7-1.2-1-2.5-1-3.8 0-1.2.3-2.2.8-3 .7-.7 1.6-1.2 2.6-1.2z"/>
        <path class="st346" d="M286.4 2639.2h4.9v7.3h-4.9z"/>
        <path class="st346" d="M351.8 2642.1l-37 14-26.6-10 37-14z"/>
        <path class="st347" d="M314.8 2656.1l37-14v2.7l-37 14-26.8-10.2.2-2.5z"/>
        <path class="st343" d="M350.9 2641.7l-36 13.6v-20h36z"/>
        <path class="st11" d="M288 2640.1c.1 0 .2 0 .3.1l26.5 8v7.1l-26.6-10.1c-.7-.8-1.2-2-1.2-3.3.1-1 .5-1.8 1-1.8z"/>
        <path class="st346" d="M325.2 2623.8l26.6 10.1-37 13.9-.8-.2-1 .4-26.7-10.1 37.9-14.5z"/>
        <path class="st347" d="M314.8 2647.8l37-13.9v2.6l-37 14-26.6-10 .3-2.6z"/>
        <path class="st347" d="M287.4 2637.7c.4 0 .8.1 1.2.2l24.6 9.3v2.7l-25.5-9.7c-.1 0-.2-.1-.3-.1-.5 0-.9.8-.9 1.8 0 1.9 1.1 3.6 2.1 4l24.6 9.4v2.7l-25.5-9.8c-1.1-.4-2-1.3-2.7-2.5-.7-1.2-1-2.5-1-3.8 0-1.2.3-2.2.8-3 .7-.7 1.6-1.2 2.6-1.2zm8.7-3.5c1.6 3.9 10.1 6.9 20.2 6.9 11.3 0 20.5-3.7 20.5-8.4 0-3.9-6.6-7.2-15.6-8.1l-25.1 9.6z"/>
        <path class="st348" d="M300 2615.5v14.7c0 3.9 7.4 7 16.5 7s16.5-3.1 16.5-7v-14.7h-33z"/>
        <path class="st349" d="M349.7 2633.9h-7.6l2-7.8h3.6z"/>
        <path class="st348" d="M316.5 2638.4c-4.6 0-9-.8-12.2-2.2-3.6-1.5-5.6-3.7-5.6-6v-14.7c0-.7.6-1.2 1.4-1.2H333c.8 0 1.4.5 1.4 1.2v14.7c0 2.3-2 4.5-5.6 6-3.4 1.4-7.7 2.2-12.3 2.2z"/>
        <path class="st344" d="M334.3 2626.3v-10h-35.7v10l13.4 5c2.4.9 6.4.9 8.8 0l13.5-5z"/>
        <path class="st11" d="M320.4 2623.9c-2.2.8-5.6.8-7.8 0l-24.5-9.1c-2.2-.8-2.2-2.1 0-2.9l24.5-9.1c2.2-.8 5.6-.8 7.8 0l24.5 9.1c2.2.8 2.2 2.1 0 2.9l-24.5 9.1z"/>
        <path class="st345" d="M320.4 2623.9c-2.2.8-5.6.8-7.8 0l-24.5-9.1c-2.2-.8-2.2-2.1 0-2.9l24.5-9.1c2.2-.8 5.6-.8 7.8 0l24.5 9.1c2.2.8 2.2 2.1 0 2.9l-24.5 9.1z"/>
        <path class="st350" d="M344.9 2613.4l-24.5 7.4c-2.2.6-5.6.6-7.8 0l-24.5-7.4c-.6-.2-1.1-.4-1.3-.7-.6.7-.2 1.5 1.3 2.1l24.5 9.1c2.2.8 5.6.8 7.8 0l24.5-9.1c1.5-.6 2-1.4 1.3-2.1-.2.3-.7.5-1.3.7z"/>
        <path class="st348" d="M316.1 2612.2c-.7 0-1.6.5-1.6 1.1 0 .6.5 1.1 1.2 1.1l28.1 1.1 1.1-.4c1.2-.5 1.8-1.1 1.6-1.7h-.3l-30.1-1.2z"/>
        <path class="st345" d="M316.5 2625.7c-1.7 0-3.2-.2-4.4-.7l-24.5-9.1c-2.1-.8-2.4-1.9-2.4-2.5s.3-1.8 2.4-2.5l24.5-9.1c1.2-.4 2.8-.7 4.4-.7s3.2.2 4.4.7l24.5 9.1c2.1.8 2.4 1.9 2.4 2.5s-.3 1.8-2.4 2.5l-24.5 9.1c-1.2.5-2.8.7-4.4.7zm-28.6-12.3c.1.1.3.2.7.4l24.5 9.1c.9.3 2.1.5 3.4.5 1.3 0 2.5-.2 3.4-.5l24.5-9.1c.4-.1.6-.3.7-.4-.1-.1-.3-.2-.7-.4l-24.5-9.1c-.9-.3-2.1-.5-3.4-.5-1.3 0-2.5.2-3.4.5l-24.5 9.1c-.4.2-.6.3-.7.4z"/>
        <path class="st349" d="M346.1 2626.2c-.7 0-1.2-.5-1.2-1.1v-11h-29.2c-.7 0-1.2-.5-1.2-1.1 0-.6.5-1.1 1.2-1.1h30.4c.7 0 1.2.5 1.2 1.1v12.1c.1.6-.5 1.1-1.2 1.1z"/>
        <ellipse class="st349" cx="345.9" cy="2625.5" rx="2.8" ry="2.6"/>
        <text transform="translate(257.76 2722.8)">
          <tspan x="0" y="0" class="st92 st90 st325">Student</tspan><tspan x="-22.9" y="24.5" class="st92 st90 st325">Scholarships</tspan>
        </text>
      </g>
    </g>
    <g id="tent-car">
      <path class="st16" d="M544.9 3356.4l-54.4 31.4 21.9 12.8 54.9-31.5z"/>
      <g class="st14">
        <path class="st231" d="M533.3 3395.8c0 2.8-1.9 6.1-4.3 7.5-2.4 1.4-4.3.3-4.3-2.5s1.9-6.1 4.3-7.5c2.3-1.3 4.3-.2 4.3 2.5z"/>
        <path class="st231" d="M526.1 3391.6c1.2-.7 2.3-.8 3.1-.3l3.1 2c-.8-.5-2-.3-3.2.4-2.4 1.4-4.3 4.7-4.3 7.5 0 1.4.4 2.1 1.1 2.5l-2.8-1.7c-.8-.5-1.3-1.4-1.3-2.8-.1-2.9 1.9-6.2 4.3-7.6z"/>
      </g>
      <g class="st14">
        <path class="st231" d="M566 3377c0 2.7-1.9 6.1-4.3 7.5-2.4 1.4-4.3.3-4.3-2.5s1.9-6.1 4.3-7.5c2.3-1.3 4.3-.2 4.3 2.5z"/>
        <path class="st11" d="M561.7 3382c1.2-.7 2.2-2.4 2.2-3.8s-1-2-2.2-1.2c-1.2.7-2.2 2.4-2.2 3.8s.9 1.9 2.2 1.2z"/>
        <path class="st231" d="M558.8 3372.8c1.2-.7 2.3-.8 3.1-.3l3.1 2c-.8-.5-2-.3-3.2.4-2.4 1.4-4.3 4.7-4.3 7.5 0 1.4.4 2.1 1.1 2.5l-2.8-1.8c-.8-.5-1.3-1.4-1.3-2.8-.1-2.8 1.9-6.1 4.3-7.5z"/>
      </g>
      <path class="st351" d="M502.2 3387.5v1.6l18.1 10.8v-1.6c0-1.9-.2-3.1 1.4-4.3l7.3-6c1.6-1.2 4.2-3.8 4.9-5.9l1.1-3c.7-2.1 2-4.5 3.6-5.4l17.2-9.9c1.6-.9 3.3-.4 3.7 1.1l.4 1.3s1.3 1.9 3.6 1.5l5.9-2.2-17.4-10.1c-.5-.3-1.2-.3-1.9 0l-1.6.7-6.5-3.8c-.7-.4-1.7-.4-2.7.2l-17.1 9.9c-1.6.9-3.5 3.4-4.3 5.4l-1.1 3c-.7 2.1-2.7 4.7-4.2 5.9l-7.3 5.4c-1.8 1.1-3.1 3.5-3.1 5.4z"/>
      <path class="st352" d="M529.8 3386.7c1.6-1.2 3.5-3.8 4.2-5.9l1.1-3c.7-2.1 2.7-4.5 4.3-5.4l17.2-9.9c1.6-.9 3.3-.4 3.7 1.1l.4 1.6c.4 1.5 2.1 2.2 3.7 1.6l3-1.3c1.6-.7 2.9.3 2.9 2.1v2.3c-.1 0-.1.1-.2.1l-1 .6c-.6.4-1.2 1.3-1.2 2v1.1c0 .6.4.9.9.8l-2.8 1.6c0-3.2-2.3-4.5-5.1-2.9s-5 5.5-5 8.7l-21.7 12.6c0-3.2-2.3-4.5-5.1-2.9s-5 5.5-5 8.7l-3.3 1.9c.5-.5.9-1.2.9-1.8v-1.1c0-.7-.5-1-1.2-.7l-.8.5v-1.6c0-1.8 1.3-4.3 2.9-5.5l7.2-5.3z"/>
      <path class="st10" d="M536.1 3377.8l-1.9 6.4c0 .1 0 .3.1.4.1 0 .1.1.2.1h.2l11.9-6.8c.1-.1.2-.2.2-.3v-7.3c0-.1-.1-.2-.2-.3s-.2-.1-.3 0l-6.9 4c-1.3.5-2.8 2.4-3.3 3.8zm12.4-9.1v7.3c0 .1.1.2.2.3h.4l6.3-3.6c.1-.1.2-.2.2-.3v-7.3c0-.1-.1-.2-.2-.3-.1-.1-.2-.1-.3 0l-6.3 3.6c-.3.1-.3.2-.3.3zm7.2-4.2v7.3c0 .1.1.2.2.3h.4l3.3-1.9c.1-.1.2-.2.2-.4l-1.2-4.7c-.2-.7-.8-1.2-1.6-1.2-.3 0-.7.1-1 .2-.2.2-.3.3-.3.4zm-40.6 10.6c0 .1.1.2.2.2l14.6 8.5h.2c.1 0 .2 0 .3-.1 1-1.2 1.9-2.7 2.3-3.9.2-.6.3-1.1.6-1.6l.5-1.4c.1-.2.2-.5.3-.7.1-.2 0-.3-.1-.4l-14.7-8.5c-.1 0-.2-.1-.3 0-.1 0-.2.1-.2.2-.1.2-.2.5-.3.7l-1.1 3c-.4 1.2-1.2 2.6-2.2 3.9-.1-.1-.2 0-.1.1z"/>
      <path class="st232" d="M546.3 3377.5v-7.3l-6.9 4c-1.1.6-2.5 2.4-3 3.8l-1.9 6.4 11.8-6.9zm2.5-1.4l6.3-3.7v-7.3l-6.3 3.6v7.4zm7.3-4.2l3.3-1.9-1.2-4.7c-.2-.9-1.2-1.2-2.2-.7l.1 7.3z"/>
      <path class="st233" d="M552.4 3376.8l1.5-.9c.3-.2.5-.5.5-.8 0-.3-.2-.4-.5-.3l-1.5.9c-.3.2-.5.5-.5.8.1.3.3.4.5.3zm-9.8 5.7l1.5-.9c.3-.1.5-.5.5-.8 0-.3-.2-.4-.5-.3l-1.5.9c-.3.2-.5.5-.5.8 0 .3.2.4.5.3z"/>
      <path class="st232" d="M515.4 3375.1c1-1.2 1.8-2.7 2.2-3.9l1.1-3c.1-.2.2-.5.3-.7l14.7 8.5c-.1.3-.2.5-.3.8l-.5 1.4c-.2.5-.4 1-.6 1.6-.4 1.2-1.3 2.6-2.3 3.8l-14.6-8.5z"/>
      <path class="st233" d="M515.1 3394.8c0-.5.3-.7.7-.4l2.2 1.3c.4.2.7.8.7 1.3s-.3.7-.7.4l-2.2-1.3c-.4-.3-.7-.9-.7-1.3zm-12.4-7.3c0-.5.3-.6.7-.4l2.2 1.3c.4.2.7.8.7 1.3s-.3.7-.7.4l-2.2-1.3c-.4-.2-.7-.8-.7-1.3z"/>
      <path class="st11" d="M528.9 3400.9c1.2-.7 2.2-2.4 2.2-3.8s-1-1.9-2.2-1.2c-1.2.7-2.2 2.4-2.2 3.8 0 1.3 1 1.9 2.2 1.2z"/>
      <path class="st14 st352" d="M569.1 3370.6c-.6.4-1.2 1.3-1.2 2v1.1c0 .6.4.9.9.8.1 0 .2-.1.3-.1l1-.6c.6-.4 1.2-1.3 1.2-2v-1.1c0-.7-.4-1-1-.8-.1 0-.1.1-.2.1l-1 .6zm-49.4 28.4c-.6.4-1.2 1.3-1.2 2v1.1c0 .7.5 1 1.2.7l1-.6c.1-.1.2-.1.3-.2.5-.4.9-1.2.9-1.8v-1.1c0-.7-.5-1-1.2-.7l-.8.5-.2.1z"/>
      <path class="st351" d="M501.2 3390.9v1.1c0 .4.1.6.3.7 5.8 3.4 11.6 6.7 17.4 10.1-.2-.1-.3-.4-.3-.7v-1.1c0-.7.5-1.6 1.2-2l-17.4-10.1c-.7.3-1.2 1.2-1.2 2z"/>
      <path class="st11" d="M507.9 3396.2v-1.8l4 2.3-.1 1.8z"/>
    </g>
    <g id="tent">
      <path class="st16" d="M456.7 3349.6l26.4-15.3 26.4 15.3-26.4 15.3z"/>
      <path class="st14 st351" d="M478.4 3331.7l28-16.3-18.6 14.5-28 16.2z"/>
      <path class="st351" d="M466.4 3355l26.4-15.3 26.4 15.2-26.4 15.3z"/>
      <path class="st352" d="M473.8 3359.3l9.8 5.6 27-15.7-9.9-5.7z"/>
      <path class="st353" d="M466.4 3355l26.4-15.3-1.3-12-26.4 15.3z"/>
      <path class="st29" d="M494.8 3360.8l26.4-15.3-2 9.4-26.4 15.3z"/>
      <path class="st237" d="M479.7 3333.3l15.1 27.5-2 9.4-7.4-4.2-5.8-21.9-5.8 15.2-7.4-4.3-2-11.8z"/>
      <path class="st14 st20" d="M478.4 3331.7l28-16.3 16.7 31.9-28 16.2z"/>
      <path class="st354" d="M479.6 3342.6v1.5l5.8 21.9 2 1.1z"/>
      <path class="st11" d="M479.6 3343.6l-8.4 15 2.6.7 5.8-15.2 5.8 21.9-.9.8z"/>
    </g>
    <g id="tent-tree">
      <path class="st16" d="M593.8 3431.8c-.4.9-1.8 1.8-3.4 2.2l-.4.1-.4.1c-.7 0-1.1 0-1.5-.2l-23.7-14.1c-.5 1.5-1.7 3-3.7 4.1-5.2 3.1-13.7 3.1-19 0-4.9-2.9-5.2-7.5-1-10.6-1.3-.4-2.5-.8-3.5-1.4-5.3-3.1-5.3-8.2-.1-11.3 5.2-3.1 13.7-3.1 19 0 1 .6 1.8 1.3 2.5 2.1 5.2-2.5 12.9-2.4 17.8.6 3.9 2.3 4.9 5.6 3.1 8.5.8.2 1.6.4 2.3.8 2.2 1.3 2.2 3.5 0 4.8-.6.3-1.2.6-1.9.7v4.9l13.4 8c.6-.2.7.2.5.7zm-24-15.2l6 3.5v-2.3c-.7-.2-1.3-.4-1.8-.7-.5-.3-.9-.7-1.3-1.1-1 .3-1.9.5-2.9.6z"/>
      <path class="st17" d="M593.5 3430c2 1.2 2 3.1 0 4.2-1.8 1.1-4.8 1.2-6.8.2-.2-.1-.3-.2-.5-.2-.2-.1-.3-.2-.4-.3-1.6-1.2-1.5-2.9.4-4 2-1.1 5.3-1.1 7.3.1z"/>
      <path class="st18" d="M607.5 3354.3c.6-1.8.9-3.7.9-5.7 0-10.2-8.3-18.5-18.5-18.5s-18.5 8.3-18.5 18.5c0 2 .3 3.9.9 5.7-9.2 1.1-16.4 8.9-16.4 18.4 0 10.2 8.3 18.5 18.5 18.5 6.5 0 12.2-3.3 15.5-8.4 3.3 5.1 9 8.4 15.5 8.4 10.2 0 18.5-8.3 18.5-18.5 0-9.5-7.2-17.4-16.4-18.4z"/>
      <path class="st19" d="M605.4 3391.2c10.2 0 18.5-8.3 18.5-18.5 0-9.5-7.2-17.3-16.4-18.4.6-1.8.9-3.7.9-5.7 0-10.2-8.3-18.5-18.5-18.5v52.8c3.3 5 9 8.3 15.5 8.3z"/>
      <path class="st17" d="M584.7 3340H595v92.1h-10.3z"/>
      <path class="st18" d="M607.5 3318.9c.6-1.8.9-3.7.9-5.7 0-10.2-8.3-18.5-18.5-18.5s-18.5 8.3-18.5 18.5c0 2 .3 3.9.9 5.7-9.2 1.1-16.4 8.9-16.4 18.4 0 10.2 8.3 18.5 18.5 18.5 6.5 0 12.2-3.3 15.5-8.4 3.3 5.1 9 8.4 15.5 8.4 10.2 0 18.5-8.3 18.5-18.5 0-9.5-7.2-17.3-16.4-18.4z"/>
      <path class="st19" d="M605.4 3355.8c10.2 0 18.5-8.3 18.5-18.5 0-9.5-7.2-17.3-16.4-18.4.6-1.8.9-3.7.9-5.7 0-10.2-8.3-18.5-18.5-18.5v52.8c3.3 5 9 8.3 15.5 8.3z"/>
      <path class="st18" d="M613.9 3357.6c0 4.4-3.5 7.9-7.9 7.9-4.3 0-7.9-3.5-7.9-7.9 0-4.3 3.5-7.9 7.9-7.9s7.9 3.5 7.9 7.9z"/>
      <path class="st17" d="M589.9 3376.7c-.8 0-1.5-.3-2.1-.9-1.2-1.2-1.2-3.1 0-4.2l15.8-15.8c1.2-1.2 3.1-1.2 4.2 0 1.2 1.2 1.2 3.1 0 4.2l-15.8 15.8c-.6.6-1.4.9-2.1.9z"/>
      <circle class="st18" cx="604.6" cy="3386.8" r="6.2"/>
      <path class="st17" d="M591.8 3401.8c-.6 0-1.2-.2-1.7-.7-.9-.9-.9-2.4 0-3.3l12.4-12.4c.9-.9 2.4-.9 3.3 0 .9.9.9 2.4 0 3.3l-12.4 12.4c-.4.5-.9.7-1.6.7z"/>
      <path class="st19" d="M562 3371.3c0 5 4 9 9 9s9-4 9-9-4-9-9-9-9 4-9 9z"/>
      <path class="st17" d="M589.6 3393.3c.9 0 1.8-.3 2.4-1 1.3-1.3 1.3-3.5 0-4.9l-18.2-18.1c-1.3-1.3-3.5-1.3-4.9 0-1.3 1.3-1.3 3.5 0 4.9l18.2 18.1c.8.6 1.7 1 2.5 1z"/>
    </g>
    <g id="we-dont-stop-there">
      <text transform="translate(1098.928 3042.122)" class="st89 st90 st91">
        We Don’t Stop There
      </text>
      <text transform="translate(1098.928 3082.66)">
        <tspan x="0" y="0" class="st92 st93 st165">The tool also intends to serve student ambassadors and </tspan><tspan x="0" y="24.5" class="st92 st93 st165">coaches wishing to give their guests and parent visitors tours</tspan><tspan x="0" y="49" class="st92 st93 st165">of the campus and facilities.</tspan>
      </text>
      <g id="we-dont-icon-1">
        <defs>
          <circle id="SVGID_12_" cx="1184.4" cy="3259.4" r="59.9"/>
        </defs>
        <use xlink:href="#SVGID_12_" overflow="visible" opacity=".56" fill="#FFF"/>
        <clipPath id="SVGID_13_">
          <use xlink:href="#SVGID_12_" overflow="visible" opacity=".56"/>
        </clipPath>
        <g class="st355">
          <path class="st356" d="M1160.6 3262.7V3227c0-10.9 10.5-19.7 23.4-19.7 13 0 23.4 8.8 23.4 19.7v35.7h-46.8z"/>
          <path class="st189" d="M1205.1 3343.7c2.1-2.7 3.1-6.1 2.6-10.3-2.4-17.7 4.2-38.9 4.8-47.7.3-4.7 7.6-7.4 4.5-11.1-4.9-5.6-22.3-11.1-32-11.1s-26.1 5.5-31 11.1c-3.2 3.6 3.2 6.4 3.5 11.1.6 8.9 4.9 29.9 2.9 46.9-.6 4.8.2 8.4 1.8 11.1h42.9z"/>
          <path class="st189" d="M1162.5 3272.4c5.7 1.5 8.6 8.4 6.5 15l-12.8 40.8c-1.2 3.8-5.4 5.9-9.4 4.9s-6.6-4.9-5.8-8.8l8.6-41.9c1.4-6.8 7.2-11.5 12.9-10zm44.7-1.8c5.8-1.2 11.4 3.8 12.4 10.6l6.4 42.3c.6 3.9-2.2 7.7-6.3 8.5-4 .8-8.1-1.5-9.1-5.4l-10.7-41.4c-1.7-6.7 1.5-13.4 7.3-14.6zm3.7 73.1c-1.3-4.2-2.5-7.7-3.2-11.1h-47.4c0 1-.1 1.9-.1 2.9-.2 3-.6 5.7-1.2 8.2h51.9z"/>
          <path class="st11" d="M1171.5 3265.2l.6 13.3c.1 1.6 1.4 2.3 3 1.5l10.5-5.1 10.1 4.8c1.6.7 2.7.1 2.6-1.5l-1.1-13.3-22.3-.8-3.4 1.1z"/>
          <path class="st171" d="M1193.9 3268.1c0 7.9-19.4 7.9-19.4 0v-26c0-5.1 3-9.3 6.8-9.3h5.9c3.7 0 6.7 4.2 6.7 9.3v26z"/>
          <path class="st172" d="M1164.2 3241.4c.2 1.3 1.5 2.2 2.9 2 1.4-.2 2.4-1.4 2.2-2.7l-1-7.2c-.2-1.3-1.5-2.2-2.9-2-1.4.2-2.4 1.4-2.2 2.7l1 7.2z"/>
          <path class="st173" d="M1165.5 3238.4c.1.5.5.8 1 .8.4-.1.8-.5.7-1l-.6-4.2c-.1-.5-.5-.8-1-.8-.5.1-.8.5-.7 1l.6 4.2z"/>
          <path class="st171" d="M1203.8 3242.1c-.2 1.3-1.5 2.2-2.9 2-1.4-.2-2.4-1.4-2.2-2.7l1-7.2c.2-1.3 1.5-2.2 2.9-2 1.4.2 2.4 1.4 2.2 2.7l-1 7.2z"/>
          <path class="st173" d="M1202.1 3239.1c-.1.5-.5.8-.9.7-.5-.1-.8-.5-.7-1l.6-4.2c.1-.5.5-.8.9-.8.5.1.8.5.7 1l-.6 4.3z"/>
          <path class="st172" d="M1168.6 3227.3c6.7 0 12.6-2.7 15.9-6.6 3.2 3.9 8.9 6.5 15.5 6.6 1.2 3.3 1.9 7 1.9 11 0 13.5-7.9 24.4-17.7 24.4-9.8 0-17.7-10.9-17.7-24.4 0-4 .7-7.7 1.9-11h.2z"/>
          <path class="st171" d="M1186 3243.2c-.7-1.7-2.2-7.4-2.2-12.1v-9.8c.2-.2.4-.5.6-.7 3.2 3.9 8.9 6.5 15.5 6.6 1.2 3.3 1.9 7 1.9 11 0 13.5-7.9 24.4-17.7 24.4h-.3s2.9-2.7 0-7.4c-.9-1.5 0-8 0-8 0-2.2 3.1-1.8 2.2-4z"/>
          <path class="st175" d="M1189.8 3251.9c-1 .3-1.4 4-6 3.7-4.3-.2-4.5-3.9-5.6-4.3.8-.1 1.8-4.1 6.1-3.8 4.1.2 4.6 3.9 5.5 4.4z"/>
          <path class="st358" d="M1181.4 3251.5c1.2.3 2.2.8 2.6 1.4.5-.5 1.5-1 2.7-1.1-1.2-.3-2.2-.8-2.6-1.4-.5.5-1.5.9-2.7 1.1z"/>
          <path class="st359" d="M1188.3 3235.9c0 1.4 2.1.8 4.7.9 2.6.1 4.7.9 4.7-.4 0-1.4-2-2.6-4.6-2.7-2.6-.2-4.8.8-4.8 2.2z"/>
          <path class="st174" d="M1189.2 3235.9c0-1.1 1.8-.5 3.9-.3 2.2.1 3.9-.4 3.9.7s-1.8 1.9-4 1.8c-2.1-.2-3.9-1.2-3.8-2.2z"/>
          <ellipse class="st359" cx="1192.7" cy="3235.6" rx="1.4" ry="1.7"/>
          <path class="st359" d="M1170.4 3235.9c0 1.4 2.1.8 4.7.9 2.6.1 4.7.9 4.7-.4 0-1.4-2-2.6-4.6-2.7-2.6-.2-4.8.8-4.8 2.2z"/>
          <path class="st174" d="M1171.2 3235.9c0-1.1 1.8-.5 3.9-.3 2.2.1 3.9-.4 3.9.7s-1.8 1.9-4 1.8c-2.1-.2-3.8-1.2-3.8-2.2z"/>
          <ellipse class="st359" cx="1174.8" cy="3235.6" rx="1.4" ry="1.7"/>
          <path class="st189" d="M1165 3230.5v3.2s1-.1 1.3 1.2c.3 1.3.5 2.8 1 4.9.5 2 1.1 3.7 4.2 3.9 3.1.2 6.1 0 7.7 0 1.6 0 3.1-2 3.7-4.6.5-2.4 1.2-3.2 1.6-3.5.3-.2.7-.2.9 0 .4.2 1.1 1 1.7 3.5.6 2.6 2.2 4.5 3.8 4.5 1.6 0 4.6.2 7.7 0 3.1-.3 3.7-1.9 4.1-4 .5-2 .7-3.6.9-4.9.3-1.3 1.2-1.2 1.2-1.2v-3.2s-10.2-.1-13.9.1c-3.8.3-3.2.9-4.1 1.3-.9.4-1.9.5-1.9.5s-1 0-1.9-.4c-.9-.4-.4-1-4.2-1.3-3.6-.2-13.8 0-13.8 0zm24.1 1.9c2.8-.4 9.9-.4 11.5-.3.8.1 2.1-.4 1.9 2.4-.1 1.5-.2 2-.4 3-.3 2.1-1 4.1-2.4 4.4-2 .4-6.4.5-8 .6-2.5 0-3.2-2-4-4.5-.7-2.4-1.1-5.2 1.4-5.6zm-19.7-.1c1.6-.1 8.7-.2 11.5.2 2.5.4 2.2 3.2 1.4 5.7-.8 2.5-1.4 4.5-3.9 4.5-1.6 0-6-.1-8-.5-1.4-.3-2.2-2.3-2.5-4.4-.2-1-.3-1.5-.4-3-.2-2.9 1-2.4 1.9-2.5z"/>
          <path class="st169" d="M1216.4 3343.7c-1.5-7.1-.9-11.9 4.3-13.5 1.2-.4 4.4 1.4 5.6 8 .3 1.4.4 3.3.4 5.4h-10.3z"/>
          <path class="st170" d="M1226.6 3343.7c0-2.2-.2-4.1-.4-5.4-1.2-6.6-4.4-8.4-5.6-8-.1 0-.2.1-.3.1 3.2.9 4.6 6.8 5.1 13.4h1.2z"/>
          <path class="st189" d="M1214.4 3343.7l-4-17.4c-1.2-5.1 1.8-8.6 5.9-9.5 4.1-.9 8.9 2.9 9.6 8.1 0 0 1 9.6 2.1 18.8h-13.6z"/>
          <path class="st175" d="M1162.4 3343.7c1.1-16.2 3.9-56.6 3.9-56.6l42.9 3s-2.5 35.9-3.7 53.6h-43.1z"/>
          <path class="st360" d="M1167.5 3343.7c-1.6-17.7-4.9-53.3-4.9-53.3l42.8-4s3.8 41.6 5.3 57.3h-43.2z"/>
          <path class="st11" d="M1164.9 3343.7c-.3-17.9-.8-53.1-.8-53.1l43-.7s.6 36.1.8 53.8h-43z"/>
          <path class="st175" d="M1163.4 3343.7c1.2-18 3.6-52.8 3.6-52.8l42.9 3s-2.2 31.3-3.4 49.8h-43.1z"/>
          <path class="st169" d="M1199.4 3315c1.2-4 3.6-2.5 7.6-4 4-1.6 4.3-3.8 4.8-1.9s-.6 3.4-4.5 4.5-.7 4.8-3.5 5c-2.6.1-4.4-3.6-4.4-3.6zm-4.9 13.6s-15.3 0-24.8 1.6-15.6.9-17.2-5.6c-.3-1.4 2-5 9.7-5.9 7.7-.9 28.8 2.3 28.8 2.3 6.8.8 7.8 7.6 3.5 7.6z"/>
          <path class="st170" d="M1194.2 3321.2s-24.3-3.5-32-2.6c-7.7.9-10 4.5-9.7 5.9 0 .1.1.2.1.3 3-8.9 38.9-2.9 38.9-2.9 2.9.6 4-.5 2.7-.7z"/>
          <path class="st169" d="M1193.2 3328.6c11 .2 17.6 2.5 16.9-.9-.5-2.2 2.1-1.3 1.4-3.6-.6-2.3 1.5-1.2.3-3.8-1.5-3.4.9-1.1-.4-3.9-1.4-2.8-7.3-.3-10.3-1.6-1-.5-1.5.1-1.9 1-.8 1.7-1.5 4.8-6.1 5.4-7.1.7-2.9 7.3.1 7.4z"/>
          <path class="st170" d="M1199.4 3315c0 4.4-2.1 6.4-5.7 7.2-1.6.2-3.9-.5-4.6-.9.6-.7 2.2-.2 3.8-.4 4.6-.6 5.3-3.7 6.1-5.4.2-.1.3-.3.4-.5z"/>
          <path class="st189" d="M1187.7 3319.1c-9.7-.8-34.9-2.8-34.9-2.8-6.3-.5-11.8 3.4-12 8.7-.2 5.3 5.1 9.6 11.4 9.4 0 0 26.1-.5 35.4-.7v-14.6z"/>
        </g>
        <text transform="translate(1144.562 3362.183)">
          <tspan x="0" y="0" class="st92 st90 st361">Student</tspan><tspan x="-28.2" y="25.8" class="st92 st90 st361">Ambassadors</tspan>
        </text>
      </g>
      <g id="we-dont-icon-2">
        <defs>
          <circle id="SVGID_14_" cx="1391" cy="3259.4" r="59.9"/>
        </defs>
        <use xlink:href="#SVGID_14_" overflow="visible" opacity=".56" fill="#FFF"/>
        <clipPath id="SVGID_15_">
          <use xlink:href="#SVGID_14_" overflow="visible" opacity=".56"/>
        </clipPath>
        <g class="st362">
          <path class="st363" d="M1423.2 3327.7c.1-8.8.5-18.7 1.4-22.8 2.4-11.5 11.8-17.3 11.3-23.2-1.4-13.1-28.7-18.3-48.4-16.5-19.7 1.9-50.2 10.6-37.6 23.2 4.7 4.7 11.2 6.2 13.8 19.5.7 3.3.4 11.9.1 19.9h59.4z"/>
          <path class="st171" d="M1404.2 3270.9c0 10.8-25.3 10.8-25.3 0v-24.6c0-4.9 3.9-8.8 8.8-8.8h7.7c4.9 0 8.8 3.9 8.8 8.8v24.6z"/>
          <path class="st177" d="M1365.7 3234c0 12.9 11.1 23.4 24.7 23.4s24.7-10.5 24.7-23.4c0-12.9-1-23.4-24.7-23.4-25.3 0-24.7 10.5-24.7 23.4z"/>
          <path class="st172" d="M1366.9 3247.1c.2 1.4 1.6 2.4 3.2 2.2 1.5-.2 2.6-1.6 2.4-3l-1.1-7.9c-.2-1.4-1.6-2.4-3.2-2.2-1.5.2-2.6 1.6-2.4 3l1.1 7.9z"/>
          <path class="st173" d="M1369.3 3243.8c.1.5.5.9 1 .8.5-.1.8-.6.8-1.1l-.7-4.6c-.1-.5-.5-.9-1-.8-.5.1-.8.6-.8 1.1l.7 4.6z"/>
          <path class="st171" d="M1414 3247.8c-.2 1.4-1.6 2.4-3.2 2.2-1.5-.2-2.6-1.6-2.4-3l1.1-7.9c.2-1.4 1.6-2.4 3.2-2.2 1.5.2 2.6 1.6 2.4 3l-1.1 7.9z"/>
          <path class="st173" d="M1411.6 3244.6c-.1.5-.5.9-1 .8-.5-.1-.8-.6-.8-1.1l.7-4.6c.1-.5.5-.9 1-.8.5.1.8.6.8 1.1l-.7 4.6z"/>
          <path class="st172" d="M1388.6 3224.6c19.3 0 20.4 9.3 20.5 9.3.9 3 1.4 6.4 1.4 9.8 0 14.8-9 26.8-20 26.8s-20-12-20-26.8c0-5.9-1.5-11.4.9-15.8 2.9-5.7 10-2.9 17.2-3.3z"/>
          <path class="st364" d="M1376.5 3239.3c0 .9 2 .5 4.6.6 2.5.1 4.6.6 4.6-.3 0-.9-2-1.7-4.5-1.8-2.6-.1-4.6.6-4.7 1.5z"/>
          <path class="st174" d="M1377.4 3239.3c0-.7 1.7-.3 3.9-.2 2.1.1 3.9-.2 3.8.5 0 .7-1.8 1.3-3.9 1.2-2.2-.1-3.9-.7-3.8-1.5z"/>
          <ellipse class="st364" cx="1380.9" cy="3239.1" rx="1.4" ry="1.2"/>
          <path class="st171" d="M1390 3224.6c21-3.6 19.1 4.6 20.5 9.3.4 4 0 6.4 0 9.8 0 14.8-9 26.8-20 26.8h-.5v-45.9z"/>
          <path class="st364" d="M1395.3 3240.1c0 .9 2 .5 4.6.6 2.5.1 4.6.6 4.6-.3 0-.9-2-1.7-4.5-1.8-2.6-.1-4.7.6-4.7 1.5z"/>
          <path class="st174" d="M1396.1 3240.1c0-.7 1.7-.3 3.9-.2 2.1.1 3.9-.2 3.8.5 0 .7-1.8 1.3-3.9 1.2-2.1-.1-3.8-.8-3.8-1.5z"/>
          <ellipse class="st364" cx="1399.6" cy="3239.9" rx="1.4" ry="1.2"/>
          <path class="st173" d="M1390.5 3270.5c-9.7 0-17.8-9.3-19.6-21.7 1.2 1.1 3.9 3.5 8 4.5 3.1.8 5.5-1.1 10.6-1.4 4.4-.2 7.2 1.7 10.2 1.1 5.3-1.1 7.9.3 10.5-4.2-1.9 12.4-10 21.7-19.7 21.7z"/>
          <path class="st186" d="M1390 3251.9c4.1-.1 6.7 1.7 9.7 1.1 5.3-1.1 8.7-1 10.5-4.2-1.8 12.4-9.9 21.7-19.6 21.7-.2 0-1.2-.1-.5 0 3.7-2.2-.1-18.6-.1-18.6z"/>
          <path class="st171" d="M1384.2 3258.4c-.1 2.1 3 .9 6.1 1 3.1.1 5 1.5 5.1-.6.1-2.1-.5-3.8-5.4-3.9-5-.3-5.7 1.4-5.8 3.5z"/>
          <path class="st175" d="M1385.7 3257.1c0 .5 1.8.3 3.9.4 2.2.1 3.9.4 4-.1 0-.5-1.7-1-3.9-1-2.2-.2-4 .2-4 .7z"/>
          <path class="st172" d="M1392.2 3239.2c.6 5.3 2.6 8.2 2.6 10.4 0 2.2-2.2 3.7-3.9 3.7-1.6 0-5.5-1.3-4.7-4.5.8-3.2 2.3-8.4 2.3-9.5 0-2.2 3.5-2.2 3.7-.1z"/>
          <path class="st173" d="M1391.9 3247.5c-1.6-5.5-1.5-9.7-1.5-9.7 1.2-.3 1.6-.1 1.7 1.1.6 5.3 2.7 8.5 2.7 10.7 0 2.2-2.2 3.7-3.9 3.7-.3 0-.6 0-.9-.1 0 0 3.5-.5 1.9-5.7z"/>
          <path class="st177" d="M1365.9 3234.4c0 12.9 11.1 23.4 24.7 23.4s24.7-10.5 24.7-23.4c0-12.9-1-23.4-24.7-23.4-25.4 0-24.7 10.5-24.7 23.4z"/>
          <path class="st172" d="M1367.1 3247.4c.2 1.4 1.6 2.4 3.2 2.2 1.5-.2 2.6-1.6 2.4-3l-1.1-7.9c-.2-1.4-1.6-2.4-3.2-2.2-1.5.2-2.6 1.6-2.4 3l1.1 7.9z"/>
          <path class="st173" d="M1369.5 3244.2c.1.5.5.9 1 .8.5-.1.8-.6.8-1.1l-.7-4.6c-.1-.5-.5-.9-1-.8-.5.1-.8.6-.8 1.1l.7 4.6z"/>
          <path class="st171" d="M1414.1 3248.2c-.2 1.4-1.6 2.4-3.2 2.2-1.5-.2-2.6-1.6-2.4-3l1.1-7.9c.2-1.4 1.6-2.4 3.2-2.2 1.5.2 2.6 1.6 2.4 3l-1.1 7.9z"/>
          <path class="st173" d="M1411.7 3244.9c-.1.5-.5.9-1 .8-.5-.1-.8-.6-.8-1.1l.7-4.6c.1-.5.5-.9 1-.8.5.1.8.6.8 1.1l-.7 4.6z"/>
          <path class="st172" d="M1388.7 3224.9c19.3 0 20.4 9.3 20.5 9.3.9 3 1.4 6.4 1.4 9.8 0 14.8-9 26.8-20 26.8s-20-12-20-26.8c0-5.9-1.5-11.4.9-15.8 3-5.6 10-2.8 17.2-3.3z"/>
          <path class="st364" d="M1376.7 3239.7c0 .9 2 .5 4.6.6 2.5.1 4.6.6 4.6-.3 0-.9-2-1.7-4.5-1.8-2.6-.1-4.7.6-4.7 1.5z"/>
          <path class="st174" d="M1377.5 3239.7c0-.7 1.7-.3 3.9-.2 2.1.1 3.9-.2 3.8.5 0 .7-1.8 1.3-3.9 1.2-2.1-.1-3.8-.8-3.8-1.5z"/>
          <ellipse class="st364" cx="1381" cy="3239.5" rx="1.4" ry="1.2"/>
          <path class="st171" d="M1390.1 3225c21-3.6 19.1 4.6 20.5 9.3.4 4 0 6.4 0 9.8 0 14.8-9 26.8-20 26.8h-.5V3225z"/>
          <path class="st364" d="M1395.4 3240.5c0 .9 2 .5 4.6.6 2.5.1 4.6.6 4.6-.3 0-.9-2-1.7-4.5-1.8-2.5-.1-4.6.6-4.7 1.5z"/>
          <path class="st174" d="M1396.3 3240.5c0-.7 1.7-.3 3.9-.2 2.1.1 3.9-.2 3.8.5 0 .7-1.8 1.3-3.9 1.2-2.2-.1-3.9-.8-3.8-1.5z"/>
          <ellipse class="st364" cx="1399.8" cy="3240.3" rx="1.4" ry="1.2"/>
          <path class="st173" d="M1390.6 3270.9c-9.7 0-17.8-9.3-19.6-21.7 1.2 1.1 3.9 3.5 8 4.5 3.1.8 5.5-1.1 10.6-1.4 4.4-.2 7.2 1.7 10.2 1.1 5.3-1.1 7.9.3 10.5-4.2-1.8 12.3-9.9 21.7-19.7 21.7z"/>
          <path class="st186" d="M1390.1 3252.3c4.1-.1 6.7 1.7 9.7 1.1 5.3-1.1 8.7-1 10.5-4.2-1.8 12.4-9.9 21.7-19.6 21.7-.2 0-1.2-.1-.5 0 3.8-2.2-.1-18.6-.1-18.6z"/>
          <path class="st171" d="M1384.3 3258.7c-.1 2.1 3 .9 6.1 1 3.1.1 5 1.5 5.1-.6.1-2.1-.5-3.8-5.4-3.9-4.9-.2-5.7 1.5-5.8 3.5z"/>
          <path class="st175" d="M1385.9 3257.4c0 .5 1.8.3 3.9.4 2.2.1 3.9.4 4-.1 0-.5-1.7-1-3.9-1-2.2-.1-4 .2-4 .7z"/>
          <path class="st172" d="M1392.4 3239.5c.6 5.3 2.6 8.2 2.6 10.4 0 2.2-2.2 3.7-3.9 3.7-1.6 0-5.5-1.3-4.7-4.5.8-3.2 2.3-8.4 2.3-9.5 0-2.1 3.4-2.1 3.7-.1z"/>
          <path class="st173" d="M1392.1 3247.9c-1.6-5.5-1.5-9.7-1.5-9.7 1.2-.3 1.6-.1 1.7 1.1.6 5.3 2.7 8.5 2.7 10.7 0 2.2-2.2 3.7-3.9 3.7-.3 0-.6 0-.9-.1-.1-.1 3.4-.5 1.9-5.7z"/>
          <path class="st365" d="M1416.4 3230.3c0-14.3-11.6-25.9-26-25.9-14.3 0-26 11.6-26 25.9l-.2 5.8 2 13.1c1.1 1.4 2.6 5.2 2.6 5.7 0 .4.1 2.4.2 3.4 0 .3.1.5.3.6.2.1.5.2.7.1h.1s.1 0 .1-.1c-.3-.8-.3-1-.3-1.7s-.2-9.2-.2-10.7-.4-5.2-.9-7.5-.7-9.2 4-11.2 14.6-2.3 17.6-2.3c3 0 12.9.3 17.6 2.3 4.7 2 4.5 8.9 4 11.2-.5 2.3-.9 6.1-.9 7.5s-.2 9.9-.2 10.7c0 .7 0 .9-.3 1.7 0 0 .1 0 .1.1h.1c.2.1.5 0 .7-.1.2-.1.3-.4.3-.6.1-1.1.2-3 .2-3.4 0-.5 1.4-4.3 2.6-5.7l2-13.1-.2-5.8z"/>
          <path class="st366" d="M1412.4 3246.6c0-1.2.4-4.9.9-7.3.6-2.5.9-10.2-4.7-12.7-5.4-2.3-16.8-2.4-18.1-2.4-1.3 0-12.7.1-18.1 2.4-5.6 2.4-5.3 10.1-4.7 12.7.5 2.3.9 6 .9 7.3 0 .5.5 8.7.7 12 .1.1.1.2.2.3.2.1.5.2.7.1h.1s.1 0 .1-.1c-.3-.8-.3-1-.3-1.7s-.2-9.2-.2-10.7-.4-5.2-.9-7.5-.7-9.2 4-11.2 14.6-2.3 17.6-2.3c3 0 12.9.3 17.6 2.3 4.7 2 4.5 8.9 4 11.2-.5 2.3-.9 6.1-.9 7.5s-.2 9.9-.2 10.7c0 .7 0 .9-.3 1.7 0 0 .1 0 .1.1h.1c.2.1.5 0 .7-.1.1-.1.2-.2.2-.3 0-3.3.5-11.5.5-12z"/>
          <path class="st367" d="M1380.7 3263.7c-.4 0-.8-.3-.9-.7-.6-2.9-4.1-18.8-4.1-18.8l1.8-.4s3.4 16 4.1 18.8c.1.5-.2 1-.7 1.1h-.2zm19.1-46.1c-3.2-.5-6.4-.9-9.4-.9s-6.3.3-9.4.9c-.4.1-.7.4-.7.9v3.9c3.4-.6 6.9-1 10.2-1 3.2 0 6.8.4 10.2 1v-3.9c-.1-.5-.4-.9-.9-.9z"/>
          <path class="st367" d="M1418.1 3247.5c-.5 0-.9-.4-.9-.9v-12.3c0-1.8-.6-4-4.7-6-4.4-2.1-14.3-4.4-22-4.4-7.7 0-17.6 2.3-22 4.4-4.1 2-4.7 4.1-4.7 6v12.3c0 .5-.4.9-.9.9s-.9-.4-.9-.9v-12.3c0-3.4 1.8-5.8 5.7-7.7 4.6-2.2 14.9-4.6 22.8-4.6 8 0 18.2 2.4 22.8 4.6 3.9 1.9 5.7 4.3 5.7 7.7v12.3c0 .5-.4.9-.9.9z"/>
          <path class="st367" d="M1400.2 3263.7h-.2c-.5-.1-.8-.6-.7-1.1.6-2.9 4.1-18.8 4.1-18.8l1.8.4s-3.4 16-4.1 18.8c-.1.4-.5.7-.9.7z"/>
          <path class="st368" d="M1417.3 3245.6c-9.4-.8-19.3-.8-24.6-.7h-4.6c-5.3 0-15.3-.1-24.5.7-.4 0-.9-.2-1-.7l-2.2-7.5c-.1-.5.1-1 .6-1.2.5-.1 1 .1 1.2.6l2 6.7c9.2-.8 18.7-.7 24-.7h4.6c5.2 0 14.8-.1 24 .7l2-6.7c.1-.5.7-.8 1.2-.6.5.1.8.7.6 1.2l-2.2 7.5c-.3.5-.7.7-1.1.7z"/>
          <path class="st368" d="M1416.7 3250.6c-9.4-.8-18.9-.8-24.1-.7h-4.6c-5.1 0-14.7-.1-24 .7-.5 0-.9-.3-1-.8l-.4-3.1c-.1-.5.3-1 .8-1.1.5-.1 1 .3 1.1.8l.3 2.2c9.1-.8 18.3-.7 23.3-.7h4.6c5 0 14.2-.1 23.3.7l.3-2.2c.1-.5.5-.9 1.1-.8.5.1.9.5.8 1.1l-.4 3.1c-.2.5-.6.8-1.1.8z"/>
          <path class="st368" d="M1390.4 3263.8c-9.4 0-12.8-.1-16-.5-3.7-.5-6.8-1.5-8.3-8.9-1.3-7.1-3.5-23.8-3.6-23.9-.1-.5.3-1 .8-1.1.5-.1 1 .3 1.1.8 0 .2 2.2 16.8 3.5 23.8 1.3 6.7 3.8 7.1 6.7 7.4 3.1.4 6.5.5 15.8.5s12.7-.1 15.8-.5c2.9-.4 5.4-.7 6.7-7.4 1.3-7 3.5-23.7 3.5-23.8.1-.5.5-.9 1.1-.8.5.1.9.5.8 1.1 0 .2-2.2 16.9-3.6 23.9-1.4 7.5-4.6 8.5-8.3 8.9-3.2.4-6.6.5-16 .5z"/>
          <g class="st58">
            <path class="st369" d="M1380.6 3225.1c1.3-.2 2.5-.4 3.8-.5v-5.8c0-1-.8-1.9-1.9-1.9-1 0-1.9.9-1.9 1.9v6.3z"/>
            <path class="st370" d="M1380.6 3222.6v2.5c1.3-.2 2.5-.4 3.8-.5v-2.5c-1.3.1-2.6.3-3.8.5z"/>
          </g>
          <radialGradient id="SVGID_16_" cx="7066.061" cy="13983.263" r="15.819" gradientTransform="matrix(.086 0 0 .086 771.274 2009.252)" gradientUnits="userSpaceOnUse">
            <stop offset="0" stop-color="#C2B48C"/>
            <stop offset="1" stop-color="#9F6F41"/>
          </radialGradient>
          <circle class="st371" cx="1382.5" cy="3218.8" r="1.4"/>
          <path class="st372" d="M1382.3 3220.1h.4v-2.5h-.4v2.5z"/>
          <path class="st372" d="M1381.8 3218.8v.2h1.3v-.4h-1.3v.2z"/>
          <g class="st58">
            <path class="st369" d="M1400.2 3225.1c-1.3-.2-2.5-.4-3.8-.5v-5.8c0-1 .8-1.9 1.9-1.9 1 0 1.9.9 1.9 1.9v6.3z"/>
            <path class="st370" d="M1400.2 3222.6v2.5c-1.3-.2-2.5-.4-3.8-.5v-2.5c1.3.1 2.6.3 3.8.5z"/>
          </g>
          <radialGradient id="SVGID_17_" cx="-12751.563" cy="13983.263" r="15.825" gradientTransform="matrix(-.086 0 0 .086 295.335 2009.252)" gradientUnits="userSpaceOnUse">
            <stop offset="0" stop-color="#C2B48C"/>
            <stop offset="1" stop-color="#9F6F41"/>
          </radialGradient>
          <circle class="st373" cx="1398.3" cy="3218.8" r="1.4"/>
          <path class="st372" d="M1398.5 3220.1h-.4v-2.5h.4v2.5z"/>
          <path class="st372" d="M1399 3218.8v.2h-1.3v-.4h1.3v.2z"/>
          <path class="st169" d="M1437.9 3327.7c1.4-.4 3-.5 4.8 0h-4.8zm-80.1 0c2.1-9 5.9-24.9 5.9-24.9-5.7-.5-12.6-.5-17.4-3.2 0 0-2.6 20-3.6 28.1h15.1z"/>
          <path class="st363" d="M1359.3 3277c-5.5-1-11.5-1-12.4 6.1l-.7 16.5c4.8 2.7 11.7 2.6 17.4 3.2l2.6-11c1.7-7-1.4-13.8-6.9-14.8z"/>
          <path class="st169" d="M1448.8 3327.7c0-.2-.1-.4-.2-.6l-10-30.1c-5.2 2.5-11 6.2-16.5 6.4 0 0 7.2 16.1 10.9 24.2h15.8z"/>
          <path class="st363" d="M1421.5 3277.3c-5.2 2-6.9 9.3-3.9 15.8l4.6 10.3c5.5-.3 11.3-3.9 16.5-6.4l-2.7-15.4c-2.3-6.7-9.3-6.3-14.5-4.3z"/>
          <path class="st169" d="M1346.6 3327.7c.9-.4 1.8-.7 3-.9.7-.1 1.7.1 2.9.9h-5.9z"/>
          <path class="st170" d="M1352.4 3327.7c-1.1-.8-2.2-1-2.9-.9-.1 0-.3.1-.4.1.7.2 1.2.4 1.8.8h1.5z"/>
        </g>
        <text transform="translate(1346.174 3362.183)">
          <tspan x="0" y="0" class="st92 st90 st361">Coaches </tspan><tspan x="-7" y="25.8" class="st92 st90 st361">&amp; Recruits</tspan>
        </text>
      </g>
      <g id="we-dont-icon-3">
        <defs>
          <circle id="SVGID_18_" cx="1586.8" cy="3259.4" r="59.9"/>
        </defs>
        <use xlink:href="#SVGID_18_" overflow="visible" opacity=".56" fill="#FFF"/>
        <clipPath id="SVGID_19_">
          <use xlink:href="#SVGID_18_" overflow="visible" opacity=".56"/>
        </clipPath>
        <g class="st374">
          <ellipse class="st375" cx="1596.5" cy="3281" rx="27.8" ry="19.5"/>
          <path class="st190" d="M1628.9 3323.3c1.3-13.5 3.4-28.8 3.4-35.5 0-12.8-16.2-23.1-36.2-23.1-20 0-36.2 10.3-36.2 23.1 0 6.7 2.1 22 3.4 35.5h65.6z"/>
          <path class="st191" d="M1597 3277.1l-6.9 2 4.2 9.8 6.4.1 2.7-10.5z"/>
          <path class="st191" d="M1587.6 3323.3c.8-8.1 1.7-16.4 2.8-20.9 2.4-10.8 4.7-14.8 4.7-14.8s3.9-2.6 5.3.3 8.8 11 7.1 28.3c-.2 2.5-.4 4.9-.5 7.2h-19.4z"/>
          <path class="st376" d="M1581.7 3283.1c.1 2 1.6 2.9 3.4 1.9l9.5-5.2c1.4-.8 3.8-.8 5.2 0l9 4.8c1.8 1 3.2.1 3-2l-1.3-17.2-12.1-5.5-17.5 6 .8 17.2z"/>
          <path class="st375" d="M1598.8 3323.3c4.5-19.1 12.5-56 10.5-59.6 5.2 1.1 26.1 14.7 26.7 15.1 16.7 13.4-1.2 9.4-2.3 21.5-.8 8.8-2 16.8-3.1 23h-31.8zm-2.5 0c-3.4-12.5-8.3-31.2-10.3-37-2.9-8.5-6-17.4-3.4-22-5.2 1.1-26.1 14.7-26.7 15.1-16.7 13.4 1.2 9.4 2.3 21.5.6 7.1 1.3 15 2 22.5h36.1z"/>
          <path class="st375" d="M1629.6 3323.3c-2.8-12-7.1-30.7-7.1-30.7-1.2-5 5.2-11.2 9.8-12.3 4.7-1.1 9.4 2 10.5 7 0 0 5.9 25.5 8.4 36.1h-21.6z"/>
          <path class="st182" d="M1651.2 3323.3c-4-15.6-9-28.1-9-28.1 2.8 8.9 3.8 19.1 5 28.1h4z"/>
          <path class="st375" d="M1524.9 3301.7c1.1 5.1 6.5 7.8 12.2 6.1l26.1-7.9c5.6-1.7 9.3-7.2 8.2-12.3-1.1-5.1-6.9-11.9-12.5-10.2l-26.1 7.9c-5.6 1.7-8.9 11.3-7.9 16.4z"/>
          <path class="st191" d="M1613.9 3306.5l.1-.1 7.5-8.2 5.1 9.6"/>
          <path class="st375" d="M1647.2 3323.3c-2.1-1.3-4.5-2.1-6.5-2.2-2.5-.1-4.7.7-6.4 2.2h12.9z"/>
          <path class="st182" d="M1647.2 3323.3c-1-.6-2-1.1-3-1.5l1.2 1.5h1.8z"/>
          <path class="st195" d="M1603.7 3323.3c3.9-7 11.4-20.5 11.4-20.5l-4.4-5.4 5.9-2.1-.8-23.8 2.7 24.1-4.6 2.7 3.4 4.2s-8.7 13.9-13.2 21h-.4zm-14.6 0c-3.8-6.8-11.7-21.1-11.7-21.1l4.4-5.4-5.9-2.1.8-23.8-2.7 24.1 4.6 2.7-3.4 4.2s9.2 14.7 13.5 21.6h.4z"/>
          <path class="st171" d="M1608.8 3268.6c0 10.9-25.6 10.9-25.6 0v-24.9c0-4.9 4-8.9 8.9-8.9h7.8c4.9 0 8.9 4 8.9 8.9v24.9z"/>
          <path class="st173" d="M1580.6 3225.9c4.6 0 8.9-1.3 12.5-3.4 14.7-7.5 11.3 9.5 19.3 9.5h.3c.9 3.1 1.3 6.5 1.3 10 0 15.1-8.6 27.3-19.2 27.3s-19.1-12.2-19.1-27.3c0-6 1.4-11.5 3.7-16 .4-.1.8-.1 1.2-.1z"/>
          <path class="st185" d="M1616.9 3236.9c-3.1 15.1-8.4 27.1-21.4 27.1-13 0-19.9-8.1-22.5-23.3-4.8-28.5 9.5-33 22.5-33s27.7-1.1 21.4 29.2z"/>
          <path class="st172" d="M1571.2 3244.5c.2 1.4 1.6 2.4 3.2 2.2 1.6-.2 2.7-1.6 2.4-3l-1.2-8c-.2-1.4-1.6-2.4-3.2-2.2-1.6.2-2.7 1.6-2.4 3l1.2 8z"/>
          <path class="st173" d="M1573.6 3241.2c.1.5.5.9 1.1.8.5-.1.8-.6.8-1.1l-.7-4.6c-.1-.5-.5-.9-1.1-.8-.5.1-.9.6-.8 1.1l.7 4.6z"/>
          <path class="st171" d="M1618.7 3245.3c-.2 1.5-1.6 2.4-3.2 2.2-1.6-.2-2.7-1.6-2.5-3l1.2-8c.2-1.4 1.6-2.4 3.2-2.2 1.6.2 2.7 1.6 2.4 3l-1.1 8z"/>
          <path class="st173" d="M1616.3 3242c-.1.5-.5.9-1 .8-.5-.1-.9-.6-.8-1.1l.7-4.6c.1-.5.6-.9 1.1-.8.5.1.9.6.8 1.1l-.8 4.6z"/>
          <path class="st172" d="M1579.8 3225.2c4.9 0 9.4-1.2 13.2-3.4 15.5-7.4 12 9.4 20.4 9.4h.4c.9 3.1 1.4 6.4 1.4 9.9 0 15-9 27.1-20.2 27.1s-20.2-12.1-20.2-27.1c0-6 1.4-11.5 3.9-15.9h1.1z"/>
          <path class="st185" d="M1581 3236.7c0 .9 2.1.5 4.6.6 2.6.1 4.6.6 4.6-.3 0-.9-2-1.8-4.5-1.8-2.5-.1-4.6.6-4.7 1.5z"/>
          <path class="st174" d="M1581.7 3236.7c0-.7 1.8-.3 3.9-.2 2.1.1 3.9-.2 3.9.5s-1.8 1.3-3.9 1.2c-2.2-.1-3.9-.7-3.9-1.5z"/>
          <ellipse class="st185" cx="1585.2" cy="3236.5" rx="1.4" ry="1.2"/>
          <path class="st171" d="M1594.2 3221.6c20-10.7 11.6 9.4 19.2 9.4.1 0 1.8.1 1.9.1.9 3.1-.2 6.3-.2 9.8 0 15-9 27.1-20.2 27.1h-.5l-.2-46.4z"/>
          <path class="st185" d="M1599.8 3237.5c0 .9 2.1.5 4.6.6 2.6.1 4.6.6 4.6-.3.1-1-1.5-1.7-4.5-1.9-2.6 0-4.7.7-4.7 1.6z"/>
          <path class="st174" d="M1600.7 3237.5c0-.7 1.8-.3 3.9-.2 2.1.1 3.9-.2 3.9.5s-1.8 1.3-4 1.2c-2.2-.1-3.9-.8-3.8-1.5z"/>
          <ellipse class="st185" cx="1604.2" cy="3237.3" rx="1.4" ry="1.2"/>
          <path class="st171" d="M1601.6 3253c-.1-2.8-4.1-.9-8.2-.7-4.1.1-6.8-1.5-6.7 1.2.1 2.8 1 5 7.6 4.8 6.6-.2 7.4-2.5 7.3-5.3z"/>
          <path class="st175" d="M1599.7 3254.9c0-.7-2.4-.3-5.3-.2-2.9.1-5.3-.2-5.3.5s2.4 1.1 5.3 1c3 0 5.3-.6 5.3-1.3z"/>
          <path class="st172" d="M1596.7 3236.6c.6 5.4 2.6 8.3 2.6 10.5 0 2.2-2.3 3.8-3.9 3.8-1.7 0-5.5-1.3-4.7-4.6.8-3.2 2.3-8.5 2.3-9.6 0-2.2 3.4-2.2 3.7-.1z"/>
          <path class="st173" d="M1596.4 3245c-1.6-5.5-1.5-9.8-1.5-9.8 1.2-.3 1.6-.1 1.8 1.1.6 5.4 2.7 8.6 2.7 10.8 0 2.2-2.3 3.8-3.9 3.8-.3 0-.6 0-1-.1-.1-.1 3.5-.6 1.9-5.8zm13.7-11.5c-6.8-2.9-11.6 2.6-12.4.7-.5-1.2 2.3-2.3 5.7-2.5 3.5-.2 6 .4 6.7 1.8zm-29.1-1.4c7-2.2 11.3 3.8 12.2 1.9.6-1.2-2.1-2.5-5.5-3-3.3-.5-5.9-.2-6.7 1.1z"/>
          <path class="st377" d="M1578.1 3253.9c.6 1.4 0 3-1.2 3.5l-8.7 3.7c-1.3.5-2.7-.2-3.3-1.6l-9.7-24.3c-.6-1.4 0-3 1.2-3.5l8.7-3.7c1.2-.5 2.7.2 3.3 1.6l9.7 24.3z"/>
          <path class="st189" d="M1576.7 3253.9c.6 1.4 0 3-1.2 3.5l-8.7 3.7c-1.2.5-2.7-.2-3.3-1.6l-9.7-24.3c-.6-1.4 0-3 1.2-3.5l8.7-3.7c1.3-.5 2.7.2 3.3 1.6l9.7 24.3z"/>
          <path class="st169" d="M1559.3 3256.3s-9.3 9.3-16.3 13.7c-7 4.4-10.2 8.7-5.8 14.8 1 1.3 5.3 2.7 10.7-1.2 5.4-3.9 15.9-18.7 15.9-18.7 3.4-4.9-1.8-11.2-4.5-8.6z"/>
          <path class="st170" d="M1563.8 3264.8s-10.4 14.8-15.9 18.7c-5.4 3.9-9.7 2.6-10.7 1.2-.1-.1-.1-.2-.2-.3 9.1 5.1 25.9-21.2 25.9-21.2 1.4-2.1 1.5.6.9 1.6z"/>
          <path class="st169" d="M1561.7 3247.5c4.2 5.8 5.3 9.6 4.6 13.8-.7 4.1-6 7.4-8.8 1.2 0 0-4.4-11.6-4.1-13.7.3-2.1 1.5-4.3 2.5-6.2.9-1.8 4.7 3.4 5.8 4.9z"/>
          <path class="st170" d="M1562.2 3254.6c-2.1-1.4-1.8-3.5.3-6 3.5 5.2 4.4 8.8 3.8 12.6-.5 3.4-4.3 6.2-7.1 3.6 4.6 1.2 8.5-6.5 3-10.2z"/>
          <path class="st169" d="M1555.6 3243.6c1-2.4 3.9-9.2 3.9-9.2l7.4-2s.5 4.5-2.2 4.6c-2.7.1-3.1-.2-3.1-.2s1.1 4.2-1.4 7.8c-1.2 1.5-5.4 1-4.6-1z"/>
          <path class="st170" d="M1560.6 3236.9c0-.6-.6-1.3 1.4-.9 1.6.3 3.5 0 4.9-2.4-.1 1.3-.5 3.2-2.2 3.3-2.7.1-3.1-.2-3.1-.2s1.1 4.2-1.4 7.8c-.5.7-1.6.9-2.5.6 3.4-1.3 3-7.6 2.9-8.2z"/>
          <path class="st169" d="M1557.6 3244.9c2.3-1.3 8.7-5.1 8.7-5.1l7.2 2.8s-2.3 3.9-4.5 2.4-2.3-2-2.3-2-1.6 4-5.8 5.4c-2 .6-5.2-2.4-3.3-3.5z"/>
          <path class="st170" d="M1565.6 3242.5c.3-.5.3-1.4 1.7.1 1.1 1.2 2.9 2.1 5.4 1-.9 1-2.3 2.3-3.8 1.3-2.2-1.5-2.3-2-2.3-2s-1.6 4-5.8 5.4c-.9.3-1.8-.2-2.3-1 3.4 1 6.8-4.3 7.1-4.8z"/>
          <path class="st169" d="M1559.6 3246.8c2.7-.5 10.4-1.9 10.4-1.9l6.1 5.3s-3.6 3-5.3.7c-1.7-2.3-1.6-2.8-1.6-2.8s-3 3.4-7.6 3.2c-2.2 0-4.3-4-2-4.5z"/>
          <path class="st170" d="M1568.3 3247.3c.5-.4.8-1.3 1.6.7.6 1.6 2.1 3.1 5 2.9-1.2.7-3.1 1.4-4.2 0-1.7-2.3-1.6-2.8-1.6-2.8s-3 3.4-7.6 3.2c-1 0-1.7-.9-1.9-1.8 2.9 2.2 8.2-1.8 8.7-2.2z"/>
          <path class="st169" d="M1561.1 3249.7c2.5.1 9.4.3 9.4.3l4.2 5.8s-3.7 1.9-4.7-.4-.8-2.8-.8-2.8-3.3 2.4-7.2 1.4c-1.9-.4-3-4.3-.9-4.3z"/>
          <path class="st170" d="M1568.6 3251.8c.5-.2.9-1 1.3.9.3 1.5 1.2 3.1 3.7 3.5-1.2.4-3 .7-3.6-.8-1-2.3-.8-2.8-.8-2.8s-3.3 2.4-7.2 1.4c-.8-.2-1.3-1.1-1.3-2 2 2.5 7.4.1 7.9-.2z"/>
          <path class="st190" d="M1536.2 3291.6c-3-2.2-4-6.1-2.1-8.6l15.4-20.9c1.9-2.6 5.9-2.8 8.9-.6 3 2.2 6.5 7.5 4.6 10.1l-15.4 20.9c-1.9 2.5-8.4 1.3-11.4-.9z"/>
          <path class="st375" d="M1526.1 3305.4c-4.1-3-5.1-8.7-2.2-12.7l17.8-24.2c3-4 8.7-4.8 12.8-1.9 4.1 3 8.5 10.6 5.6 14.6l-17.8 24.2c-2.8 4.1-12 3-16.2 0z"/>
          <path class="st182" d="M1554.1 3266.4c1.8 7.4 1.4 15-2.9 22.6-7.1 11.3-10.6 15.7-23.6 17.4 4.6 2.1 11.8 2.5 14.4-1l17.8-24.2c3-4-1.4-11.6-5.6-14.6.1-.1 0-.1-.1-.2z"/>
        </g>
        <text transform="translate(1555.412 3362.183)">
          <tspan x="0" y="0" class="st92 st90 st361">Visiting</tspan><tspan x="-27.2" y="25.8" class="st92 st90 st361">Parent Tours</tspan>
        </text>
      </g>
    </g>
  </svg>
</template>

<style>

body {
  background-color: #f7f7f7;
  height: 2000px;
}
</style>
