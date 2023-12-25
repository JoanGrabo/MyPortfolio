    .skills{
        margin-top: -150px;
        div{
            grid-template-columns: repeat(6,1fr);
            gap: 20px;
            .skill-el{
                padding: 25px;
                &:hover{
                    transform: scale(1.05);
                    transition: 300ms;
                }
                img{
                    width: 100%;
                    height: 100%;
                    max-height: 80px;
                    object-fit: contain;
                }
            }
        }
        h3{
            color: $primaryColor;
            margin-top: 75px;
            border-left: 5px solid $primaryColor;
            padding-left: 20px;
        }
    }
    .section{
        min-height: 100vh;
        padding: 0;
        >article{
            grid-column: 3 / 11;
        }
        article:has(.elements){
            display: grid;
            grid-template-columns: repeat(8,1fr);
            gap: 20px;
            h2{
                grid-column: 1 / 9;
            }
            .elements{
                grid-column: 2 / 8;
            }
        }
    }