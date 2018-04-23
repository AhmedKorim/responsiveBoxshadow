# responsiveBoxshadow
 creats a responsive css shadow
 
 ## EXAMPLE: 
 ### sass input:
 
         .card{
            @include resshad(1,4,transparentize(black, .8),20,0);
        
        }

### css output :

        @media (max-width: 576px) {
          .card {
            box-shadow: 0.48px 1.92px 0px 9.6px rgba(0, 0, 0, 0.2);
          }
        }
        @media (min-width: 576px) {
          .card {
            box-shadow: 0.48px 1.92px 0px 9.6px rgba(0, 0, 0, 0.2);
          }
        }
        @media (min-width: 768px) {
          .card {
            box-shadow: 0.64px 2.56px 0px 12.8px rgba(0, 0, 0, 0.2);
          }
        }
        @media (min-width: 992px) {
          .card {
            box-shadow: 0.83px 3.31px 0px 16.53px rgba(0, 0, 0, 0.2);
          }
        }
        @media (min-width: 1200px) {
          .card {
            box-shadow: 1px 4px 0px 20px rgba(0, 0, 0, 0.2);
          }
        }
## usage

-import the file to your main sass file`@import`

-call the mixin `@include`

-variables on order `xOffset yOffset color blur spreed`

- note :`blur an spreed` **optional**
