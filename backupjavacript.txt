



                        //videosmortalkombar
            let videos=[
            "https://www.youtube.com/embed/P0PVHFTWajM",
            "https://www.youtube.com/embed/wkFd2aPBRvQ",
            "https://www.youtube.com/embed/K4Cr-T1KFss",
            "https://www.youtube.com/embed/f5QZHPDbceg",
            "https://www.youtube.com/embed/zbktVFky3C4",
            "https://www.youtube.com/embed/XeQryt_NU2Y",
            "https://www.youtube.com/embed/ZdC5mFHPldg",
            "https://www.youtube.com/embed/alVyFX7iQg8",
            "https://www.youtube.com/embed/f1eqbqDSgTY",
            "https://www.youtube.com/embed/8Tk8sqXlogM",
            "https://www.youtube.com/embed/Zl56jUBgbD4",
            "https://www.youtube.com/embed/J_wfivrRIs0",
            "https://www.youtube.com/embed/T9sq0Wj5PMM",
            "https://www.youtube.com/embed/aZWirlzaDOw",
            "https://www.youtube.com/embed/NYH2sLid0Zc",
            "https://www.youtube.com/embed/wcf5UAWgDl4",
            "https://www.youtube.com/embed/FnedlyPZoLI",
            "https://www.youtube.com/embed/a9pHkX7c3y8",
            "https://www.youtube.com/embed/25n8murcTQk",
            "https://www.youtube.com/embed/1ANF5X1Szn4",
            "https://www.youtube.com/embed/TqNOTLfYkmk",
            "https://www.youtube.com/embed/NBk5cSDdqDo",
            "https://www.youtube.com/embed/jP41y1P-w_g",
            "https://www.youtube.com/embed/THHY-z4zgIc",
            "https://www.youtube.com/embed/r6LwkSIKKts",
            "https://www.youtube.com/embed/QJHY4ggYCk4",
            "https://www.youtube.com/embed/Sr1bLLvsbh0",
            "https://www.youtube.com/embed/EAwWPadFsOA",
            "https://www.youtube.com/embed/SjWrERa4cy4",
            "https://www.youtube.com/embed/SAv23TpJxDI",
            "https://www.youtube.com/embed/_NMk8_o1Eoc",
            "https://www.youtube.com/embed/FnedlyPZoLI",
            "https://www.youtube.com/embed/lfaH-xiGlls",
            "https://www.youtube.com/embed/nLJ5MaGtmwE",
            "https://www.youtube.com/embed/R60rMWvb5W4",
            "https://www.youtube.com/embed/1UqU-yyH9dg",
            "https://www.youtube.com/embed/THHY-z4zgIc",
            "https://www.youtube.com/embed/NBk5cSDdqDo",
            "https://www.youtube.com/embed/JZpqp6OLe3U",
            "https://www.youtube.com/embed/CfhIzgdvYKc",
            "https://www.youtube.com/embed/JHIfHL5UgFs",
            "https://www.youtube.com/embed/w-FsjAwlybk",
            "https://www.youtube.com/embed/N7XvA9gOCxQ",
            "https://www.youtube.com/embed/GT9LYeLKgOM",
            "https://www.youtube.com/embed/tCp__6K6uwo",
            "https://www.youtube.com/embed/_hlTbEDYaNo",
            "https://www.youtube.com/embed/Mt6xSztFHBg",
            "https://www.youtube.com/embed/Sfohcjr_VaI",
            "https://www.youtube.com/embed/1UqU-yyH9dg"
            ];
            //controledovideo
            let indexe=0;
            let contador=0;
            let limiteporvideo=1;
            document.getElementById('btn').onclick=function(){
                let final=indexe+limiteporvideo;
                for(;indexe<final && indexe<videos.length;indexe++){
                    if(contador==2){
                        let div=document.createElement('div');
                        div.innerHTML=`
                           <a href="https://victorxx.github.io/hospedagem02/" target="_blank" rel="noopener noreferrer" style="
                            display: inline-block;
                            background-color: #28a745;
                            color: white;
                            padding: 12px 20px;
                            text-decoration: none;
                            border-radius: 5px;
                            font-weight: bold;
                            font-size: 1rem;
                            transition: background-color 0.3s ease;
                            ">
                            CONFERIR ESSA OPORTUNIDADE
                            </a>
                            <br>
                            <br>
                            <br>
                                 <a href="https://victorxx.github.io/diadia2/" target="_blank" rel="noopener noreferrer" style="
                            display: inline-block;
                            background-color: #28a745;
                            color: white;
                            padding: 12px 20px;
                            text-decoration: none;
                            border-radius: 5px;
                            font-weight: bold;
                            font-size: 1rem;
                            transition: background-color 0.3s ease;
                            ">
                            CONFIRA ESSA OPORTUNIDADE
                            </a>
                            <br>
                            <br>
                            <br>
                                       <a href="https://victorxx.github.io/redirecionarmdj/" target="_blank" rel="noopener noreferrer" style="
                            display: inline-block;
                            background-color: #28a745;
                            color: white;
                            padding: 12px 20px;
                            text-decoration: none;
                            border-radius: 5px;
                            font-weight: bold;
                            font-size: 1rem;
                            transition: background-color 0.3s ease;
                            ">
                            CONFIRA ESSA OPORTUNIDADE
                            </a>
                            <br>
                            <br>
                            <br>


                        `;
                        document.getElementById('video').appendChild(div);
                        contador=0;
                    }
                    let iframe=document.createElement('iframe');
                    iframe.src=videos[indexe];
                    contador++;

                    iframe.width=300;
                    iframe.height=300;
                    document.getElementById('video').appendChild(iframe);
                }
                 if (indexe >= videos.length) {
                    this.disabled = true;
                    this.innerText = "Todos os vídeos carregados";
                }
            };
  
