# IDR identification regulation

- cut
- block
- unit
- module
- element
##構造

.idr-grid-cut<header>
    |- idr-hed-block<h1> (id.tone.logotype)

.idr-grid-cut<main>  
      |- .idr-hed-block<h2> (.typography)
      |- .idr-hed-block<h3> (.anatomy)
      |- .idr-li-block<dl>
        |- <dt> (.typeface)
        |- <dd>
			|- idr-hed-unit<h4> (Overpass)
			|- .idr-list-module<ul>
				|- li*
        |- <dd>
			|- idr-hed-module<h4> (Heisei Kaku Gothic Std / 平成角ゴシック Std)
			|- .idr-list-module<ul>
				|- li*
		|- <dt>(.weight)
		|- <dd>
			|- idr-hed-module<h4> (Overpass)
			|- .idr-list-module<ul>
				|- li*
        |- <dd>
			|- idr-hed-module<h4> (Heisei Kaku Gothic Std / 平成角ゴシック Std)
			|- .idr-list-module<ul>
				|- li*
		|- <dt>(.size)
		|- <dd>
            |- .idr-list-module<ul>
                |- li*
        |- <dt> (.tracking)
		|- <dd>
            |- idr-list-module<ul>
                |- li*
        |- <dt> (.leading)
		|- <dd>
            |-idr-list-module<ul>
                |- li*
idr-grid-cut<footer>
    |- <small>

header
  |- input (id.tone.logotype)

main  
      |- h1 (.tone)
      |- h2(.color)
      |- dl
        |- dt (leihauoli.black)
        |- dd
            |- ul
                |- li*
        |- dd
            |- ul
                |- li*
		|- dt (leihauoli.gray)    
        |- dd
            |- ul
                |- li*
        |- dd
            |- ul
                |- li*

##json構造
{
    "CATEGORY": {
        "GROUP": {
            "PROPERTY" : {
                "BOARDTYPE" : "rendertype (A)",
                "KEYBOARD" : [
                      {
                        "LABEL" : "titlename (Overpass or null)",
						"KEYCHAIN" : [
                            {"KEY (weight)" : "numTitle",
							"VALUE " : value (100)}
                        ]
                      }
                ]
            }
        }
    }
}



{
	"CATEGORY":".typography",
	"GROUP": ".anatomy",
	"PROPERTY": ".typeface",
	"??" : {
		"BOARDTYPE" : "A",
		"KEYBOARD" : [
			{
				"LABEL" : "Overpass",
				"KEYCHAIN" : [
					{"KEY " : "thin", "UNIT" : "weight", "VALUE" : 100}
				]
			}
		]
	}
}   
