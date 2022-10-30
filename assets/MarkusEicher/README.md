# Proposal for Photo Gallery Collage Landingpage

### Created by: MarkusEicher

> This proposal for a landing page is based on the  
> free template "Simplistic Photo Collage" of Framer.  

Under the following link you can visit a clickable prototype  
https://frank-anxiety-905545.framer.app/

The reason why I think that a collage is the best form for  
a photographer's landing page is because it is mobile first  
and responsive. While a caroussel has a good effect on wider  
viewports, it has flaws on small phone viewports. A collage  
can be made as sophisticated as a caroussel on wider viewports  
without losing attractiveness on small devices.  

The following Screenshot shows the basic view of the three main  
viewports of the proposed design. Please notice, that the various  
pictures are not forced into a predefined roster and they can keep  
their original size. This makes them feel more natural.  

![Simplistic-Photo-Collage-Viewports](https://user-images.githubusercontent.com/83175378/198907069-5c0e855f-70e9-4dc3-88fe-fa46f180ee3a.PNG)

Another advantage when using Framer with this template is, that we  
have the option to use the components in a react project. The code  
can be generated in the Framer app and reflects changes we make in  
the design software. The following excerpt shows an example.

```jsx import type { ComponentType } from "react"
import { createStore } from "https://framer.com/m/framer/store.js@^1.0.0"
import { randomColor } from "https://framer.com/m/framer/utils.js@^0.9.0"

// Learn more: https://www.framer.com/docs/guides/overrides/

const useStore = createStore({
    background: "#0099FF",
})

export function withRotate(Component): ComponentType {
    return (props) => {
        return (
            <Component
                {...props}
                animate={{ rotate: 90 }}
                transition={{ duration: 2 }}
            />
        )
    }
}

export function withHover(Component): ComponentType {
    return (props) => {
        return <Component {...props} whileHover={{ scale: 1.05 }} />
    }
}
```
