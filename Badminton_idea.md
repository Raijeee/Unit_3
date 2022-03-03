Calculate the times the shuttle landed in every section of the court.

```.py
Screen:
    BoxLayout:
        orientation: "vertical"
        size_hint: 1,1

        BoxLayout:
            orientation:"vertical"
            size_hint: 1,.15
            MDLabel:
                text: "Singles Badminton Shuttle Counter"
                halign:"center"
                font_size: "40"

        BoxLayout:
            orientation:"vertical"
            size_hint:1,.8
            # Player A (Side A)
            BoxLayout:
                orientation: "horizontal"
                size_hint:1,1

                Button:
                    id:aback # Back line
                    size_hint: .2,1
                    text: "0"
                    font_size: "32"
                    background_color: 0, 1, 0, 1
                    on_release:
                        app.aback()

                Button:
                    id:amiddle # Middle line
                    size_hint: .7,1
                    text:"0"
                    font_size: "32"
                    background_color: 0, 1, 0, 1
                    on_release:
                        app.amiddle()
                BoxLayout:
                    orientation: "vertical"
                    size_hint:1,1
                    Button:
                        id:arightquad #Right service line
                        size_hint: 1,1
                        text:"0"
                        font_size: "32"
                        background_color: 0, 1, 0, 1
                        on_release:
                            app.arightquad()
                    Button:
                        id:aleftquad # Left service line
                        size_hint: 1,1
                        text:"0"
                        font_size: "32"
                        background_color: 0, 1, 0, 1
                        on_release:
                            app.aleftquad()

               #Player B (Side B)
                BoxLayout:
                    orientation: "vertical"
                    size_hint:1,1
                    Button:
                        id:brightquad #Right service line
                        size_hint: 1,1
                        text:"0"
                        font_size: "32"
                        background_color: 0, 1, 0, 1
                        on_release:
                            app.brightquad()

                    Button:
                        id:bleftquad # Left service line
                        size_hint: 1,1
                        text:"0"
                        font_size: "32"
                        background_color: 0, 1, 0, 1
                        on_release:
                            app.bleftquad()
                Button:
                    id:bmiddle # Middle line
                    size_hint: .7,1
                    text:"0"
                    font_size: "32"
                    background_color: 0, 1, 0, 1
                    on_release:
                        app.bmiddle()
                Button:
                    id:bback # Back line
                    size_hint: .2,1
                    text:"0"
                    font_size: "32"
                    background_color: 0, 1, 0, 1
                    on_release:
                        app.bback()


        BoxLayout:
            orientation: "vertical"
            size_hint: 1,.05
```


