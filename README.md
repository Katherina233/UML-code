# ---3-12
//类图连接代码

Skip to content
Features
Business
Explore
Pricing
This repository
Sign in or Sign up

0
0

    0

zzwennie/11-_-
Code
Issues 0
Pull requests 0
Projects 0
Pulse
Graphs
11-_-/类图2.mdl
96b0c6b on 5 Mar
@zzwennie zzwennie Add files via upload
7384 lines (7381 sloc) 194 KB

(object Petal
    version    	47
    _written   	"Rose 8.0.0303.1400"
    charSet    	134)

(object Design "Logical View"
    is_unit    	TRUE
    is_loaded  	TRUE
    attributes 	(list Attribute_Set
	(object Attribute
	    tool       	"Java"
	    name       	"IDE"
	    value      	"Internal Editor")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagName1"
	    value      	"")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagText1"
	    value      	"")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagApply1"
	    value      	"")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagName2"
	    value      	"")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagText2"
	    value      	"")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagApply2"
	    value      	"")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagName3"
	    value      	"")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagText3"
	    value      	"")
	(object Attribute
	    tool       	"Java"
	    name       	"UserDefineTagApply3"
	    value      	""))
    quid       	"39C9260C00D4"
    defaults   	(object defaults
	rightMargin 	0.250000
	leftMargin 	0.250000
	topMargin  	0.250000
	bottomMargin 	0.500000
	pageOverlap 	0.250000
	clipIconLabels 	TRUE
	autoResize 	TRUE
	snapToGrid 	TRUE
	gridX      	16
	gridY      	16
	defaultFont 	(object Font
	    size       	10
	    face       	"Arial"
	    bold       	FALSE
	    italics    	FALSE
	    underline  	FALSE
	    strike     	FALSE
	    color      	0
	    default_color 	TRUE)
	showMessageNum 	1
	showClassOfObject 	TRUE
	notation   	"Unified")
    root_usecase_package 	(object Class_Category "Use Case View"
	quid       	"39C9260C00D6"
	exportControl 	"Public"
	global     	TRUE
	logical_models 	(list unit_reference_list)
	logical_presentations 	(list unit_reference_list
	    (object UseCaseDiagram "Main"
		quid       	"39C9261001B7"
		title      	"Main"
		zoom       	100
		max_height 	28350
		max_width  	21600
		origin_x   	0
		origin_y   	0
		items      	(list diagram_item_list))))
    root_category 	(object Class_Category "Logical View"
	quid       	"39C9260C00D5"
	exportControl 	"Public"
	global     	TRUE
	subsystem  	"Component View"
	quidu      	"39C9260C00D7"
	logical_models 	(list unit_reference_list
	    (object Class "NvWa"
		quid       	"58BB9546023A")
	    (object Class "AbstractHumanFactory"
		quid       	"58BB95AB0289"
		used_nodes 	(list uses_relationship_list
		    (object Uses_Relationship
			quid       	"58BB986B014A"
			supplier   	"Logical View::Human"
			quidu      	"58BB96DC0210"))
		operations 	(list Operations
		    (object Operation "createHuman"
			quid       	"58BB95FD00A6"
			parameters 	(list Parameters
			    (object Parameter "c"
				quid       	"58BB966803C4"
				type       	"Class"
				quidu      	"39CD6AE10136"))
			result     	"Human"
			concurrency 	"Sequential"
			opExportControl 	"Public"
			uid        	0)))
	    (object Class "Human"
		quid       	"58BB96DC0210"
		operations 	(list Operations
		    (object Operation "getColor"
			quid       	"58BB97190201"
			result     	"Void   (Logical View::java::lang::Void)"
			concurrency 	"Sequential"
			opExportControl 	"Public"
			uid        	0)
		    (object Operation "talk"
			quid       	"58BB9742007B"
			result     	"void"
			concurrency 	"Sequential"
			opExportControl 	"Public"
			uid        	0)))
	    (object Class "HumanFactory"
		quid       	"58BB97600185"
		superclasses 	(list inheritance_relationship_list
		    (object Inheritance_Relationship
			quid       	"58BB98C403CB"
			supplier   	"Logical View::AbstractHumanFactory"
			quidu      	"58BB95AB0289")))
	    (object Class "BlackHuman"
		quid       	"58BB977C00BA"
		realized_interfaces 	(list realize_rel_list
		    (object Realize_Relationship
			quid       	"58BB9A210101"
			supplier   	"Logical View::Human"
			quidu      	"58BB96DC0210")))
	    (object Class "YellowHuman"
		quid       	"58BB979A030C"
		realized_interfaces 	(list realize_rel_list
		    (object Realize_Relationship
			quid       	"58BB998F0082"
			supplier   	"Logical View::Human"
			quidu      	"58BB96DC0210")))
	    (object Class "WhiteHuman"
		quid       	"58BB97C50222"
		realized_interfaces 	(list realize_rel_list
		    (object Realize_Relationship
			quid       	"58BB9A5901DC"
			supplier   	"Logical View::Human"
			quidu      	"58BB96DC0210")))
	    (object Association "$UNNAMED$0"
		quid       	"58BB97F70148"
		roles      	(list role_list
		    (object Role "$UNNAMED$1"
			quid       	"58BB97F90242"
			supplier   	"Logical View::AbstractHumanFactory"
			quidu      	"58BB95AB0289"
			is_navigable 	TRUE)
		    (object Role "$UNNAMED$2"
			quid       	"58BB97F90252"
			supplier   	"Logical View::NvWa"
			quidu      	"58BB9546023A")))
	    (object Association "$UNNAMED$3"
		quid       	"58BB982801F5"
		roles      	(list role_list
		    (object Role "$UNNAMED$4"
			quid       	"58BB982C0168"
			supplier   	"Logical View::Human"
			quidu      	"58BB96DC0210"
			is_navigable 	TRUE)
		    (object Role "$UNNAMED$5"
			quid       	"58BB982C016A"
			supplier   	"Logical View::NvWa"
			quidu      	"58BB9546023A")))
	    (object Class_Category "javax"
		is_unit    	TRUE
		is_loaded  	FALSE
		file_name  	"$FRAMEWORK_PATH\\Shared Components\\j2ee_javax.cat"
		quid       	"39C926610018")
	    (object Class_Category "java"
		is_unit    	TRUE
		is_loaded  	FALSE
		file_name  	"$FRAMEWORK_PATH\\Shared Components\\j2se_1_3_java.cat"
		quid       	"39C92661003B")
	    (object Class_Category "org"
		is_unit    	TRUE
		is_loaded  	FALSE
		file_name  	"$FRAMEWORK_PATH\\Shared Components\\j2se_1_3_org.cat"
		quid       	"39C92693036F"))
	logical_presentations 	(list unit_reference_list
	    (object ClassDiagram "Package Hierarchy"
		quid       	"39C9261001B8"
		title      	"Package Hierarchy"
		zoom       	100
		max_height 	28350
		max_width  	21600
		origin_x   	0
		origin_y   	0
		items      	(list diagram_item_list
		    (object ClassView "Class" "Logical View::HumanFactory" @1
			ShowCompartmentStereotypes 	TRUE
			IncludeAttribute 	TRUE
			IncludeOperation 	TRUE
			location   	(288, 912)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@1
			    location   	(104, 861)
			    fill_color 	13434879
			    nlines     	1
			    max_width  	368
			    justify    	0
			    label      	"HumanFactory")
			icon_style 	"Icon"
			line_color 	3342489
			fill_color 	13434879
			quidu      	"58BB97600185"
			width      	386
			height     	126
			annotation 	8
			autoResize 	TRUE)
		    (object ClassView "Class" "Logical View::BlackHuman" @2
			ShowCompartmentStereotypes 	TRUE
			IncludeAttribute 	TRUE
			IncludeOperation 	TRUE
			location   	(784, 976)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@2
			    location   	(626, 925)
			    fill_color 	13434879
			    nlines     	1
			    max_width  	316
			    justify    	0
			    label      	"BlackHuman")
			icon_style 	"Icon"
			line_color 	3342489
			fill_color 	13434879
			quidu      	"58BB977C00BA"
			width      	334
			height     	126
			annotation 	8
			autoResize 	TRUE)
		    (object ClassView "Class" "Logical View::YellowHuman" @3
			ShowCompartmentStereotypes 	TRUE
			IncludeAttribute 	TRUE
			IncludeOperation 	TRUE
			location   	(1360, 976)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@3
			    location   	(1195, 925)
			    fill_color 	13434879
			    nlines     	1
			    max_width  	330
			    justify    	0
			    label      	"YellowHuman")
			icon_style 	"Icon"
			line_color 	3342489
			fill_color 	13434879
			quidu      	"58BB979A030C"
			width      	348
			height     	126
			annotation 	8
			autoResize 	TRUE)
		    (object ClassView "Class" "Logical View::WhiteHuman" @4
			ShowCompartmentStereotypes 	TRUE
			IncludeAttribute 	TRUE
			IncludeOperation 	TRUE
			location   	(1856, 976)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@4
			    location   	(1696, 925)
			    fill_color 	13434879
			    nlines     	1
			    max_width  	320
			    justify    	0
			    label      	"WhiteHuman")
			icon_style 	"Icon"
			line_color 	3342489
			fill_color 	13434879
			quidu      	"58BB97C50222"
			width      	338
			height     	126
			annotation 	8
			autoResize 	TRUE)
		    (object ClassView "Class" "Logical View::AbstractHumanFactory" @5
			ShowCompartmentStereotypes 	TRUE
			IncludeAttribute 	TRUE
			IncludeOperation 	TRUE
			location   	(288, 496)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@5
			    location   	(25, 415)
			    fill_color 	13434879
			    nlines     	1
			    max_width  	526
			    justify    	0
			    label      	"AbstractHumanFactory")
			icon_style 	"Icon"
			line_color 	3342489
			fill_color 	13434879
			quidu      	"58BB95AB0289"
			compartment 	(object Compartment
			    Parent_View 	@5
			    location   	(25, 476)
			    font       	(object Font
				size       	10
				face       	"Arial"
				bold       	FALSE
				italics    	FALSE
				underline  	FALSE
				strike     	FALSE
				color      	0
				default_color 	TRUE)
			    icon_style 	"Icon"
			    fill_color 	13434879
			    anchor     	2
			    nlines     	2
			    max_width  	325)
			width      	544
			height     	186
			annotation 	8
			autoResize 	TRUE)
		    (object ClassView "Class" "Logical View::NvWa" @6
			ShowCompartmentStereotypes 	TRUE
			IncludeAttribute 	TRUE
			IncludeOperation 	TRUE
			location   	(288, 160)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@6
			    location   	(166, 85)
			    fill_color 	13434879
			    nlines     	1
			    max_width  	244
			    justify    	0
			    label      	"NvWa")
			icon_style 	"Icon"
			line_color 	3342489
			fill_color 	13434879
			quidu      	"58BB9546023A"
			width      	262
			height     	175
			annotation 	8
			autoResize 	TRUE)
		    (object AssociationViewNew "$UNNAMED$0" @7
			location   	(288, 324)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			stereotype 	TRUE
			line_color 	3342489
			quidu      	"58BB97F70148"
			roleview_list 	(list RoleViews
			    (object RoleView "$UNNAMED$1" @8
				Parent_View 	@7
				location   	(112, 116)
				stereotype 	TRUE
				line_color 	3342489
				quidu      	"58BB97F90242"
				client     	@7
				supplier   	@5
				line_style 	0)
			    (object RoleView "$UNNAMED$2" @9
				Parent_View 	@7
				location   	(112, 116)
				stereotype 	TRUE
				line_color 	3342489
				quidu      	"58BB97F90252"
				client     	@7
				supplier   	@6
				line_style 	0)))
		    (object ClassView "Class" "Logical View::Human" @10
			ShowCompartmentStereotypes 	TRUE
			IncludeAttribute 	TRUE
			IncludeOperation 	TRUE
			location   	(1360, 496)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@10
			    location   	(1224, 390)
			    fill_color 	13434879
			    nlines     	1
			    max_width  	272
			    justify    	0
			    label      	"Human")
			icon_style 	"Icon"
			line_color 	3342489
			fill_color 	13434879
			quidu      	"58BB96DC0210"
			compartment 	(object Compartment
			    Parent_View 	@10
			    location   	(1224, 451)
			    font       	(object Font
				size       	10
				face       	"Arial"
				bold       	FALSE
				italics    	FALSE
				underline  	FALSE
				strike     	FALSE
				color      	0
				default_color 	TRUE)
			    icon_style 	"Icon"
			    fill_color 	13434879
			    anchor     	2
			    nlines     	3
			    max_width  	234)
			width      	290
			height     	236
			annotation 	8
			autoResize 	TRUE)
		    (object AssociationViewNew "$UNNAMED$3" @11
			location   	(998, 159)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			stereotype 	TRUE
			line_color 	3342489
			quidu      	"58BB982801F5"
			roleview_list 	(list RoleViews
			    (object RoleView "$UNNAMED$4" @12
				Parent_View 	@11
				location   	(710, -17)
				stereotype 	TRUE
				line_color 	3342489
				quidu      	"58BB982C0168"
				client     	@11
				supplier   	@10
				vertices   	(list Points
				    (998, 159)
				    (1359, 159)
				    (1359, 377))
				line_style 	0)
			    (object RoleView "$UNNAMED$5" @13
				Parent_View 	@11
				location   	(710, -17)
				stereotype 	TRUE
				line_color 	3342489
				quidu      	"58BB982C016A"
				client     	@11
				supplier   	@6
				line_style 	0)))
		    (object UsesView "" @14
			stereotype 	TRUE
			line_color 	3342489
			quidu      	"58BB986B014A"
			client     	@5
			supplier   	@10
			line_style 	0)
		    (object InheritView "" @15
			stereotype 	TRUE
			line_color 	3342489
			quidu      	"58BB98C403CB"
			client     	@1
			supplier   	@5
			line_style 	0)
		    (object RealizeView "" @16
			stereotype 	TRUE
			line_color 	3342489
			quidu      	"58BB998F0082"
			client     	@3
			supplier   	@10
			line_style 	0)
		    (object RealizeView "" @17
			stereotype 	TRUE
			line_color 	3342489
			quidu      	"58BB9A210101"
			client     	@2
			supplier   	@10
			vertices   	(list Points
			    (782, 912)
			    (781, 800)
			    (1359, 800)
			    (1359, 614))
			line_style 	0)
		    (object RealizeView "" @18
			stereotype 	TRUE
			line_color 	3342489
			quidu      	"58BB9A5901DC"
			client     	@4
			supplier   	@10
			vertices   	(list Points
			    (1854, 912)
			    (1853, 800)
			    (1359, 800)
			    (1359, 614))
			line_style 	0)
		    (object NoteView @19
			location   	(1904, 496)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@19
			    location   	(1766, 436)
			    fill_color 	13434879
			    nlines     	2
			    max_width  	240
			    label      	"人类")
			line_color 	3342489
			fill_color 	13434879
			width      	300
			height     	132)
		    (object NoteView @20
			location   	(784, 1232)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@20
			    location   	(646, 1172)
			    fill_color 	13434879
			    nlines     	2
			    max_width  	240
			    label      	"黑色人种")
			line_color 	3342489
			fill_color 	13434879
			width      	300
			height     	132)
		    (object NoteView @21
			location   	(1360, 1232)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@21
			    location   	(1222, 1172)
			    fill_color 	13434879
			    nlines     	2
			    max_width  	240
			    label      	"黄色人种")
			line_color 	3342489
			fill_color 	13434879
			width      	300
			height     	132)
		    (object NoteView @22
			location   	(1856, 1248)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@22
			    location   	(1718, 1188)
			    fill_color 	13434879
			    nlines     	2
			    max_width  	240
			    label      	"白色人种")
			line_color 	3342489
			fill_color 	13434879
			width      	300
			height     	132)
		    (object NoteView @23
			location   	(496, 752)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			label      	(object ItemLabel
			    Parent_View 	@23
			    location   	(352, 686)
			    fill_color 	13434879
			    nlines     	2
			    max_width  	253
			    label      	"抽象的八卦炉")
			line_color 	3342489
			fill_color 	13434879
			width      	313
			height     	144)
		    (object AttachView "" @24
			stereotype 	TRUE
			line_color 	3342489
			client     	@5
			supplier   	@23
			line_style 	0)
		    (object AttachView "" @25
			stereotype 	TRUE
			line_color 	3342489
			client     	@10
			supplier   	@19
			line_style 	0)
		    (object AttachView "" @26
			stereotype 	TRUE
			line_color 	3342489
			client     	@2
			supplier   	@20
			line_style 	0)
		    (object AttachView "" @27
			stereotype 	TRUE
			line_color 	3342489
			client     	@3
			supplier   	@21
			line_style 	0)
		    (object AttachView "" @28
			stereotype 	TRUE
			line_color 	3342489
			client     	@4
			supplier   	@22
			line_style 	0)))
	    (object ClassDiagram "Legend"
		quid       	"39CD51840059"
		title      	"Legend"
		zoom       	100
		max_height 	28350
		max_width  	21600
		origin_x   	0
		origin_y   	0
		items      	(list diagram_item_list
		    (object NoteView @29
			location   	(224, 624)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			line_color 	3342489
			fill_color 	12632256
			width      	300
			height     	132)
		    (object NoteView @30
			location   	(704, 624)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			line_color 	3342489
			fill_color 	8421631
			width      	300
			height     	132)
		    (object NoteView @31
			location   	(1200, 624)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			line_color 	3342489
			fill_color 	12615680
			width      	300
			height     	132)
		    (object NoteView @32
			location   	(1664, 624)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			line_color 	3342489
			fill_color 	16777215
			width      	300
			height     	132)
		    (object Label @33
			location   	(81, 369)
			font       	(object Font
			    size       	12
			    face       	"Arial"
			    bold       	TRUE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			nlines     	1
			max_width  	1163
			label      	"J2EE: Java 2 Platform, Enterprise Edition - v 1.2.1")
		    (object Label @34
			location   	(96, 608)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			nlines     	1
			max_width  	268
			label      	"Abstract Class")
		    (object Label @35
			location   	(592, 608)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			nlines     	1
			max_width  	225
			label      	"Final Class")
		    (object Label @36
			location   	(1104, 608)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			nlines     	1
			max_width  	206
			label      	"Interface")
		    (object Label @37
			location   	(1552, 608)
			font       	(object Font
			    size       	10
			    face       	"Arial"
			    bold       	FALSE
			    italics    	FALSE
			    underline  	FALSE
			    strike     	FALSE
			    color      	0
			    default_color 	TRUE)
			nlines     	1
			max_width  	144
			label      	"Class")))))
    root_subsystem 	(object SubSystem "Component View"
	quid       	"39C9260C00D7"
	physical_models 	(list unit_reference_list
	    (object SubSystem "javax"
		is_unit    	TRUE
		is_loaded  	FALSE
		file_name  	"$FRAMEWORK_PATH\\Shared Components\\j2ee_javax.sub"
		quid       	"39C9266003D8")
	    (object SubSystem "java"
		is_unit    	TRUE
		is_loaded  	FALSE
		file_name  	"$FRAMEWORK_PATH\\Shared Components\\j2se_1_3_java.sub"
		quid       	"39C92661002C")
	    (object SubSystem "org"
		is_unit    	TRUE
		is_loaded  	FALSE
		file_name  	"$FRAMEWORK_PATH\\Shared Components\\j2se_1_3_org.sub"
		quid       	"39C9268C01C9"))
	physical_presentations 	(list unit_reference_list
	    (object Module_Diagram "Main"
		quid       	"39C9261001B6"
		title      	"Main"
		zoom       	100
		max_height 	28350
		max_width  	21600
		origin_x   	0
		origin_y   	0
		items      	(list diagram_item_list))))
    process_structure 	(object Processes
	quid       	"39C9260C00D8"
	ProcsNDevs 	(list
	    (object Process_Diagram "Deployment View"
		quid       	"39C9260C00DA"
		title      	"Deployment View"
		zoom       	100
		max_height 	28350
		max_width  	21600
		origin_x   	0
		origin_y   	0
		items      	(list diagram_item_list))))
    properties 	(object Properties
	attributes 	(list Attribute_Set
	    (object Attribute
		tool       	"CORBA"
		name       	"propertyId"
		value      	"809135966")
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Project"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"CreateMissingDirectories"
			value      	TRUE)
		    (object Attribute
			tool       	"CORBA"
			name       	"Editor"
			value      	("EditorType" 100))
		    (object Attribute
			tool       	"CORBA"
			name       	"IncludePath"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"StopOnError"
			value      	TRUE)
		    (object Attribute
			tool       	"CORBA"
			name       	"EditorType"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"CORBA"
				name       	"BuiltIn"
				value      	100)
			    (object Attribute
				tool       	"CORBA"
				name       	"WindowsShell"
				value      	101)))
		    (object Attribute
			tool       	"CORBA"
			name       	"PathSeparator"
			value      	"")))
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"ArrayDimensions"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"ConstValue"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"ImplementationType"
			value      	"")))
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"AdditionalIncludes"
			value      	(value Text ""))
		    (object Attribute
			tool       	"CORBA"
			name       	"CmIdentification"
			value      	(value Text "  %X% %Q% %Z% %W%"))
		    (object Attribute
			tool       	"CORBA"
			name       	"CopyrightNotice"
			value      	(value Text ""))
		    (object Attribute
			tool       	"CORBA"
			name       	"InclusionProtectionSymbol"
			value      	"AUTO GENERATE")))
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Module-Body"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"AdditionalIncludes"
			value      	(value Text ""))
		    (object Attribute
			tool       	"CORBA"
			name       	"CmIdentification"
			value      	(value Text "  %X% %Q% %Z% %W%"))
		    (object Attribute
			tool       	"CORBA"
			name       	"CopyrightNotice"
			value      	(value Text ""))
		    (object Attribute
			tool       	"CORBA"
			name       	"InclusionProtectionSymbol"
			value      	"AUTO GENERATE")))
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"Context"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"OperationIsOneWay"
			value      	FALSE)))
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"ArrayDimensions"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"CaseSpecifier"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"IsReadOnly"
			value      	FALSE)
		    (object Attribute
			tool       	"CORBA"
			name       	"Order"
			value      	"")))
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"ArrayDimensions"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"CaseSpecifier"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"GenerateForwardReference"
			value      	FALSE)
		    (object Attribute
			tool       	"CORBA"
			name       	"IsReadOnly"
			value      	FALSE)
		    (object Attribute
			tool       	"CORBA"
			name       	"Order"
			value      	"")
		    (object Attribute
			tool       	"CORBA"
			name       	"BoundedRoleType"
			value      	("AssocTypeSet" 47))
		    (object Attribute
			tool       	"CORBA"
			name       	"AssocTypeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"CORBA"
				name       	"Array"
				value      	24)
			    (object Attribute
				tool       	"CORBA"
				name       	"Sequence"
				value      	47)))))
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Uses"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"GenerateForwardReference"
			value      	FALSE)))
	    (object Attribute
		tool       	"CORBA"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Data Modeler"
		name       	"propertyId"
		value      	"809135966")
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Project"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"project"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"TableCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DomainCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"SPPackageCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"TriggerCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IndexCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ConstraintCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"StoreProcedureCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"PrimaryKeyCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ForeignKeyCounter"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"TablePrefix"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DomainPrefix"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"TriggerPrefix"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IndexPrefix"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ConstraintPrefix"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"StoreProcedurePrefix"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"PrimaryKeyPrefix"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ForeignKeyPrefix"
			value      	"")))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmItem"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DMName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsDatabase"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"TargetDatabase"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Location"
			value      	"")))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Category"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmItem"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DMName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmSchema"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmDomainPackage"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsSchema"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsDomainPackage"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsRootSchema"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsRootDomainPackage"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsSchemaPackage"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DatabaseID"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DBMS"
			value      	"")))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmItem"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DMName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsTable"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsView"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsDomain"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsSPPackage"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Synonymns"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"TableSpace"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"SourceId"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"SourceType"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"SelectClause"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsUpdatable"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"CheckOption"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"PersistToServer"
			value      	"")))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmItem"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DMName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Ordinal"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsIdentity"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsUnique"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"NullsAllowed"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DataTypeName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Length"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Scale"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ColumnType"
			value      	"Native")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ForBitData"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DefaultValueType"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DefaultValue"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"SourceId"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"SourceType"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"OID"
			value      	FALSE)))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Association"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmItem"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DMName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsRelationship"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"SourceId"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"SourceType"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"RIMethod"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ParentUpdateRule"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ParentUpdateRuleName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ParentDeleteRule"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ParentDeleteRuleName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ChildInsertRestrict"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ChildInsertRestrictName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ChildMultiplicity"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ChildMultiplicityName"
			value      	"")))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmItem"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DMName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ConstraintName"
			value      	"")))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmItem"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DMName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsConstraint"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ConstraintType"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsIndex"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsTrigger"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsStoredProcedure"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsCluster"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"TableSpace"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"FillFactor"
			value      	0)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"KeyList"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"CheckPredicate"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsUnique"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DeferalMode"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"InitialCheckTime"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"TriggerType"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsInsertEvent"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsUpdateEvent"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsDeleteEvent"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"RefOldTable"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"RefNewTable"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"RefOldRow"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"RefNewRow"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsRow"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"WhenClause"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Language"
			value      	"SQL")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ProcType"
			value      	"Procedure")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsDeterministic"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ParameterStyle"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ReturnedNull"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ExternalName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ReturnTypeName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Length"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Scale"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ForBitData"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DefaultValue"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DefaultValueType"
			value      	"")))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"default__Parameter"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Data Modeler"
			name       	"dmItem"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DMName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsInParameter"
			value      	TRUE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"IsOutParameter"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Ordinal"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DataTypeName"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Length"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"Scale"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"ForBitData"
			value      	FALSE)
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DefaultValueType"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"DefaultValue"
			value      	"")
		    (object Attribute
			tool       	"Data Modeler"
			name       	"OperationID"
			value      	"")))
	    (object Attribute
		tool       	"Data Modeler"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Data Modeler Communicator"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"framework"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Java"
		name       	"propertyId"
		value      	"809135966")
	    (object Attribute
		tool       	"Java"
		name       	"default__Project"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"RootDir"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"CreateMissingDirectories"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"StopOnError"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"UsePrefixes"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"AutoSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ShowCodegenDlg"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"JavadocDefaultAuthor"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"JavadocDefaultVersion"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"JavadocDefaultSince"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"JavadocNumAsterisks"
			value      	0)
		    (object Attribute
			tool       	"Java"
			name       	"MaxNumChars"
			value      	80)
		    (object Attribute
			tool       	"Java"
			name       	"Editor"
			value      	("EditorType" 100))
		    (object Attribute
			tool       	"Java"
			name       	"VM"
			value      	("VMType" 200))
		    (object Attribute
			tool       	"Java"
			name       	"ClassPath"
			value      	"D:\\sqljdbc4.jar")
		    (object Attribute
			tool       	"Java"
			name       	"EditorType"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"BuiltIn"
				value      	100)
			    (object Attribute
				tool       	"Java"
				name       	"WindowsShell"
				value      	101)))
		    (object Attribute
			tool       	"Java"
			name       	"VMType"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Sun"
				value      	200)
			    (object Attribute
				tool       	"Java"
				name       	"Microsoft"
				value      	201)
			    (object Attribute
				tool       	"Java"
				name       	"IBM"
				value      	202)))
		    (object Attribute
			tool       	"Java"
			name       	"InstanceVariablePrefix"
			value      	"m_")
		    (object Attribute
			tool       	"Java"
			name       	"ClassVariablePrefix"
			value      	"s_")
		    (object Attribute
			tool       	"Java"
			name       	"DefaultAttributeDataType"
			value      	"int")
		    (object Attribute
			tool       	"Java"
			name       	"DefaultOperationReturnType"
			value      	"void")
		    (object Attribute
			tool       	"Java"
			name       	"NoClassCustomDlg"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GlobalImports"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Java"
			name       	"OpenBraceClassStyle"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"OpenBraceMethodStyle"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"UseTabs"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"UseSpaces"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"SpacingItems"
			value      	3)
		    (object Attribute
			tool       	"Java"
			name       	"RoseDefaultCommentStyle"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"AsteriskCommentStyle"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"JavaCommentStyle"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"JavadocAuthor"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"JavadocSince"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"JavadocVersion"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"NotShowRoseIDDlg"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateRoseID"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateDefaultJ2EEJavadoc"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateDefaultReturnLine"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"UserDefineJavaDocTags"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ReferenceClasspath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"VAJavaWorkingFolder"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"BeanPrefix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"BeanSuffix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"RemotePrefix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"RemoteSuffix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"HomePrefix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"HomeSuffix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"LocalPrefix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"LocalSuffix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"LocalHomePrefix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"LocalHomeSuffix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"PrimaryKeyPrefix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"PrimaryKeySuffix"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBDTDLocation"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletDTDLocation"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"DefaultEJBVersion"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"DefaultServletVersion"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"SourceControl"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"SCCSelected"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"SCCProjectSourceRoot"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"SCCProjectName"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"SCCComment"
			value      	FALSE)))
	    (object Attribute
		tool       	"Java"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"Final"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Static"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateDefaultConstructor"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"ConstructorIs"
			value      	("Ctor_Set" 62))
		    (object Attribute
			tool       	"Java"
			name       	"Ctor_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"public"
				value      	62)
			    (object Attribute
				tool       	"Java"
				name       	"protected"
				value      	63)
			    (object Attribute
				tool       	"Java"
				name       	"private"
				value      	64)
			    (object Attribute
				tool       	"Java"
				name       	"package"
				value      	65)))
		    (object Attribute
			tool       	"Java"
			name       	"GenerateFinalizer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateStaticInitializer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateInstanceInitializer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateCode"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"DisableAutoSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ReadOnly"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Strictfp"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletName"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletContextRef"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"IsSingleThread"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletInitParameter"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletInitParameterNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletIsSecure"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestDispatcher"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestDispatcherPath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"DispatcherInclude"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"DispatcherForward"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletSecurityRoles"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletgetInfo"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletXMLFilePath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestAttribute"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestAttributesNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForRequestAttributes"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestParameter"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestParameterNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForRequestParameters"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletHeader"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletHeaderNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForHeaders"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletIntHeader"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletDateHeader"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletCookie"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForCookie"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletContentType"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"GenerateHTML"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Generate_XML_DD"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBCmpField"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBEnvironmentProperties"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBCnxFactory"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBReferences"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBSecurityRoles"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBNameInJAR"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionType"
			value      	("EJBSessionType_Set" 200))
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	""
				value      	200)
			    (object Attribute
				tool       	"Java"
				name       	"Stateless"
				value      	201)
			    (object Attribute
				tool       	"Java"
				name       	"Stateful"
				value      	202)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBTransactionType"
			value      	("EJBTransactionType_Set" 211))
		    (object Attribute
			tool       	"Java"
			name       	"EJBTransactionType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Container"
				value      	211)
			    (object Attribute
				tool       	"Java"
				name       	"Bean"
				value      	212)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBPersistenceType"
			value      	("EJBPersistenceType_Set" 220))
		    (object Attribute
			tool       	"Java"
			name       	"EJBPersistenceType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	""
				value      	220)
			    (object Attribute
				tool       	"Java"
				name       	"Bean"
				value      	221)
			    (object Attribute
				tool       	"Java"
				name       	"Container"
				value      	222)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBReentrant"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBVersion"
			value      	("EJBVersion_Set" 230))
		    (object Attribute
			tool       	"Java"
			name       	"EJBVersion_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"2.0"
				value      	230)
			    (object Attribute
				tool       	"Java"
				name       	"1.x"
				value      	231)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBXMLFilePath"
			value      	"")))
	    (object Attribute
		tool       	"Java"
		name       	"Default_Servlet__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"ServletName"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletContextRef"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"IsSingleThread"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletInitParameter"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletInitParameterNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletIsSecure"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestDispatcher"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestDispatcherPath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"DispatcherInclude"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"DispatcherForward"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletSecurityRoles"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletgetInfo"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"Final"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Static"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateDefaultConstructor"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"ConstructorIs"
			value      	("Ctor_Set" 62))
		    (object Attribute
			tool       	"Java"
			name       	"Ctor_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"public"
				value      	62)
			    (object Attribute
				tool       	"Java"
				name       	"protected"
				value      	63)
			    (object Attribute
				tool       	"Java"
				name       	"private"
				value      	64)
			    (object Attribute
				tool       	"Java"
				name       	"package"
				value      	65)))
		    (object Attribute
			tool       	"Java"
			name       	"GenerateFinalizer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateStaticInitializer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateInstanceInitializer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateCode"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"DisableAutoSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ReadOnly"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Strictfp"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletXMLFilePath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestAttribute"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestAttributesNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForRequestAttributes"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestParameter"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestParameterNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForRequestParameters"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletHeader"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletHeaderNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForHeaders"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletIntHeader"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletDateHeader"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletCookie"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForCookie"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletContentType"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"GenerateHTML"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Generate_XML_DD"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBCmpField"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBEnvironmentProperties"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBCnxFactory"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBReferences"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBSecurityRoles"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBNameInJAR"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionType"
			value      	("EJBSessionType_Set" 200))
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	""
				value      	200)
			    (object Attribute
				tool       	"Java"
				name       	"Stateless"
				value      	201)
			    (object Attribute
				tool       	"Java"
				name       	"Stateful"
				value      	202)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBTransactionType"
			value      	("EJBTransactionType_Set" 211))
		    (object Attribute
			tool       	"Java"
			name       	"EJBTransactionType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Container"
				value      	211)
			    (object Attribute
				tool       	"Java"
				name       	"Bean"
				value      	212)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBPersistenceType"
			value      	("EJBPersistenceType_Set" 220))
		    (object Attribute
			tool       	"Java"
			name       	"EJBPersistenceType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	""
				value      	220)
			    (object Attribute
				tool       	"Java"
				name       	"Bean"
				value      	221)
			    (object Attribute
				tool       	"Java"
				name       	"Container"
				value      	222)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBReentrant"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBVersion"
			value      	("EJBVersion_Set" 230))
		    (object Attribute
			tool       	"Java"
			name       	"EJBVersion_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"2.0"
				value      	230)
			    (object Attribute
				tool       	"Java"
				name       	"1.x"
				value      	231)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBXMLFilePath"
			value      	"")))
	    (object Attribute
		tool       	"Java"
		name       	"Http_Servlet__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestAttribute"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestAttributesNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForRequestAttributes"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestParameter"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestParameterNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForRequestParameters"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletHeader"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletHeaderNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForHeaders"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletIntHeader"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletDateHeader"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletCookie"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForCookie"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletContentType"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"GenerateHTML"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Final"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Static"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateDefaultConstructor"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"ConstructorIs"
			value      	("Ctor_Set" 62))
		    (object Attribute
			tool       	"Java"
			name       	"Ctor_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"public"
				value      	62)
			    (object Attribute
				tool       	"Java"
				name       	"protected"
				value      	63)
			    (object Attribute
				tool       	"Java"
				name       	"private"
				value      	64)
			    (object Attribute
				tool       	"Java"
				name       	"package"
				value      	65)))
		    (object Attribute
			tool       	"Java"
			name       	"GenerateFinalizer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateStaticInitializer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateInstanceInitializer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateCode"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"DisableAutoSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ReadOnly"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Strictfp"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletName"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletContextRef"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"IsSingleThread"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletInitParameter"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletInitParameterNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletIsSecure"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestDispatcher"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestDispatcherPath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"DispatcherInclude"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"DispatcherForward"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletSecurityRoles"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletgetInfo"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletXMLFilePath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"Generate_XML_DD"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBCmpField"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBEnvironmentProperties"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBCnxFactory"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBReferences"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBSecurityRoles"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBNameInJAR"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionType"
			value      	("EJBSessionType_Set" 200))
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	""
				value      	200)
			    (object Attribute
				tool       	"Java"
				name       	"Stateless"
				value      	201)
			    (object Attribute
				tool       	"Java"
				name       	"Stateful"
				value      	202)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBTransactionType"
			value      	("EJBTransactionType_Set" 211))
		    (object Attribute
			tool       	"Java"
			name       	"EJBTransactionType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Container"
				value      	211)
			    (object Attribute
				tool       	"Java"
				name       	"Bean"
				value      	212)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBPersistenceType"
			value      	("EJBPersistenceType_Set" 220))
		    (object Attribute
			tool       	"Java"
			name       	"EJBPersistenceType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	""
				value      	220)
			    (object Attribute
				tool       	"Java"
				name       	"Bean"
				value      	221)
			    (object Attribute
				tool       	"Java"
				name       	"Container"
				value      	222)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBReentrant"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBVersion"
			value      	("EJBVersion_Set" 230))
		    (object Attribute
			tool       	"Java"
			name       	"EJBVersion_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"2.0"
				value      	230)
			    (object Attribute
				tool       	"Java"
				name       	"1.x"
				value      	231)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBXMLFilePath"
			value      	"")))
	    (object Attribute
		tool       	"Java"
		name       	"Default_EJB__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"Generate_XML_DD"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBCmpField"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBEnvironmentProperties"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBCnxFactory"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBReferences"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBSecurityRoles"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBNameInJAR"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionType"
			value      	("EJBSessionType_Set" 200))
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	""
				value      	200)
			    (object Attribute
				tool       	"Java"
				name       	"Stateless"
				value      	201)
			    (object Attribute
				tool       	"Java"
				name       	"Stateful"
				value      	202)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBTransactionType"
			value      	("EJBTransactionType_Set" 211))
		    (object Attribute
			tool       	"Java"
			name       	"EJBTransactionType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Container"
				value      	211)
			    (object Attribute
				tool       	"Java"
				name       	"Bean"
				value      	212)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBPersistenceType"
			value      	("EJBPersistenceType_Set" 220))
		    (object Attribute
			tool       	"Java"
			name       	"EJBPersistenceType_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	""
				value      	220)
			    (object Attribute
				tool       	"Java"
				name       	"Bean"
				value      	221)
			    (object Attribute
				tool       	"Java"
				name       	"Container"
				value      	222)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBReentrant"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"BMP_Extend_CMP"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Final"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Static"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateDefaultConstructor"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"ConstructorIs"
			value      	("Ctor_Set" 62))
		    (object Attribute
			tool       	"Java"
			name       	"Ctor_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"public"
				value      	62)
			    (object Attribute
				tool       	"Java"
				name       	"protected"
				value      	63)
			    (object Attribute
				tool       	"Java"
				name       	"private"
				value      	64)
			    (object Attribute
				tool       	"Java"
				name       	"package"
				value      	65)))
		    (object Attribute
			tool       	"Java"
			name       	"GenerateFinalizer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateStaticInitializer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateInstanceInitializer"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateCode"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"DisableAutoSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ReadOnly"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Strictfp"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletName"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletContextRef"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"IsSingleThread"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletInitParameter"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletInitParameterNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletIsSecure"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestDispatcher"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestDispatcherPath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"DispatcherInclude"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"DispatcherForward"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletSecurityRoles"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletgetInfo"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletXMLFilePath"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestAttribute"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestAttributesNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForRequestAttributes"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestParameter"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletRequestParameterNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForRequestParameters"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletHeader"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletHeaderNames"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForHeaders"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletIntHeader"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletDateHeader"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ServletCookie"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"MethodForCookie"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"ServletContentType"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"GenerateHTML"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBSessionSync"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"EJBVersion"
			value      	("EJBVersion_Set" 230))
		    (object Attribute
			tool       	"Java"
			name       	"EJBVersion_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"2.0"
				value      	230)
			    (object Attribute
				tool       	"Java"
				name       	"1.x"
				value      	231)))
		    (object Attribute
			tool       	"Java"
			name       	"EJBXMLFilePath"
			value      	"")))
	    (object Attribute
		tool       	"Java"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"CmIdentification"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Java"
			name       	"CopyrightNotice"
			value      	(value Text ""))))
	    (object Attribute
		tool       	"Java"
		name       	"default__Module-Body"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"CmIdentification"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Java"
			name       	"CopyrightNotice"
			value      	(value Text ""))))
	    (object Attribute
		tool       	"Java"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"Abstract"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Static"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Final"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Native"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Synchronized"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"GenerateFullyQualifiedReturn"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"ReplaceExistingCode"
			value      	TRUE)
		    (object Attribute
			tool       	"Java"
			name       	"Strictfp"
			value      	FALSE)))
	    (object Attribute
		tool       	"Java"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"Final"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Transient"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Volatile"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"PropertyType"
			value      	("BeanProperty_Set" 71))
		    (object Attribute
			tool       	"Java"
			name       	"BeanProperty_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Not A Property"
				value      	71)
			    (object Attribute
				tool       	"Java"
				name       	"Simple"
				value      	72)
			    (object Attribute
				tool       	"Java"
				name       	"Bound"
				value      	73)
			    (object Attribute
				tool       	"Java"
				name       	"Constrained"
				value      	74)))
		    (object Attribute
			tool       	"Java"
			name       	"IndividualChangeMgt"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Read/Write"
			value      	("Read/Write_Set" 81))
		    (object Attribute
			tool       	"Java"
			name       	"Read/Write_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Read & Write"
				value      	81)
			    (object Attribute
				tool       	"Java"
				name       	"Read Only"
				value      	82)
			    (object Attribute
				tool       	"Java"
				name       	"Write Only"
				value      	83)))
		    (object Attribute
			tool       	"Java"
			name       	"GenerateFullyQualifiedTypes"
			value      	FALSE)))
	    (object Attribute
		tool       	"Java"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Java"
			name       	"ContainerClass"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"InitialValue"
			value      	"")
		    (object Attribute
			tool       	"Java"
			name       	"Final"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Transient"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Volatile"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"PropertyType"
			value      	("BeanProperty_Set" 71))
		    (object Attribute
			tool       	"Java"
			name       	"BeanProperty_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Not A Property"
				value      	71)
			    (object Attribute
				tool       	"Java"
				name       	"Simple"
				value      	72)
			    (object Attribute
				tool       	"Java"
				name       	"Bound"
				value      	73)
			    (object Attribute
				tool       	"Java"
				name       	"Constrained"
				value      	74)))
		    (object Attribute
			tool       	"Java"
			name       	"IndividualChangeMgt"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"Read/Write"
			value      	("Read/Write_Set" 81))
		    (object Attribute
			tool       	"Java"
			name       	"Read/Write_Set"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Java"
				name       	"Read & Write"
				value      	81)
			    (object Attribute
				tool       	"Java"
				name       	"Read Only"
				value      	82)
			    (object Attribute
				tool       	"Java"
				name       	"Write Only"
				value      	83)))
		    (object Attribute
			tool       	"Java"
			name       	"GenerateFullyQualifiedTypes"
			value      	FALSE)
		    (object Attribute
			tool       	"Java"
			name       	"IsNavigable"
			value      	TRUE)))
	    (object Attribute
		tool       	"Java"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"R2Editor"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Rose Web Publisher"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"COM"
		name       	"propertyId"
		value      	"783606378")
	    (object Attribute
		tool       	"COM"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"COM"
			name       	"TypeKinds"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"COM"
				name       	"enum"
				value      	100)
			    (object Attribute
				tool       	"COM"
				name       	"record"
				value      	101)
			    (object Attribute
				tool       	"COM"
				name       	"module"
				value      	102)
			    (object Attribute
				tool       	"COM"
				name       	"interface"
				value      	103)
			    (object Attribute
				tool       	"COM"
				name       	"dispinterface"
				value      	104)
			    (object Attribute
				tool       	"COM"
				name       	"coclass"
				value      	105)
			    (object Attribute
				tool       	"COM"
				name       	"alias"
				value      	106)
			    (object Attribute
				tool       	"COM"
				name       	"union"
				value      	107)
			    (object Attribute
				tool       	"COM"
				name       	"max"
				value      	108)
			    (object Attribute
				tool       	"COM"
				name       	"(none)"
				value      	109)))
		    (object Attribute
			tool       	"COM"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"COM"
			name       	"kind"
			value      	("TypeKinds" 109))
		    (object Attribute
			tool       	"COM"
			name       	"uuid"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"version"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"helpstring"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"helpcontext"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"attributes"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"dllname"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"alias"
			value      	"")))
	    (object Attribute
		tool       	"COM"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"COM"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"COM"
			name       	"id"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"helpstring"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"attributes"
			value      	"")))
	    (object Attribute
		tool       	"COM"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"COM"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"COM"
			name       	"id"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"helpstring"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"attributes"
			value      	"")))
	    (object Attribute
		tool       	"COM"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"COM"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"COM"
			name       	"filename"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"library"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"uuid"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"version"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"helpstring"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"helpfile"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"helpcontext"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"lcid"
			value      	"")
		    (object Attribute
			tool       	"COM"
			name       	"attributes"
			value      	"")))
	    (object Attribute
		tool       	"COM"
		name       	"default__Param"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"COM"
			name       	"attributes"
			value      	"")))
	    (object Attribute
		tool       	"COM"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"VC++"
		name       	"propertyId"
		value      	"809135966")
	    (object Attribute
		tool       	"VC++"
		name       	"default__Project"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"VC++"
			name       	"UpdateATL"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"SmartPointersOnAssoc"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"GenerateImports"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"PutImportsIn"
			value      	"stdafx.h")
		    (object Attribute
			tool       	"VC++"
			name       	"FullPathInImports"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"UseImportAttributes"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"ImportAttributes"
			value      	"no_namespace named_guids")
		    (object Attribute
			tool       	"VC++"
			name       	"ImportProjTypeLib"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"DefaultTypeLib"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"TypeLibLocation"
			value      	"")
		    (object Attribute
			tool       	"VC++"
			name       	"CompileProjTypeLib"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"IdlInterfaceAttributes"
			value      	(value Text 
|endpoint("")
|local
|object
|pointer_default()
|uuid("")
|version("")
|encode
|decode
|auto_handle
|implicit_handle("")
|code
|nocode
			))
		    (object Attribute
			tool       	"VC++"
			name       	"IdlCoClassAttributes"
			value      	(value Text 
|uuid("")
|helpstring("")
|helpcontext("")
|licensed
|version("")
|control
|hidden
|appobject
			))
		    (object Attribute
			tool       	"VC++"
			name       	"IdlCoClassInterfaceAttributes"
			value      	(value Text 
|default
|source
			))
		    (object Attribute
			tool       	"VC++"
			name       	"IdlParameterAttributes"
			value      	(value Text 
|in
|out
|retval
			))
		    (object Attribute
			tool       	"VC++"
			name       	"IdlMethodAttributes"
			value      	(value Text 
|id(1)
|helpstring("")
|call_as("")
|callback
|helpcontext("")
|hidden
|local
|restricted
|source
|vararg
			))
		    (object Attribute
			tool       	"VC++"
			name       	"IdlPropertyAttributes"
			value      	(value Text 
|id()
|helpstring("")
|call_as("")
|helpcontext("")
|hidden
|local
|restricted
|source
|vararg
|bindable
|defaultbind
|defaultcallelem
|displaybind
|immediatebind
|nonbrowseable
|requestedit
			))
		    (object Attribute
			tool       	"VC++"
			name       	"RvcPtyVersion"
			value      	"1.3")
		    (object Attribute
			tool       	"VC++"
			name       	"ModelIDStyle"
			value      	2)
		    (object Attribute
			tool       	"VC++"
			name       	"DocStyle"
			value      	1)
		    (object Attribute
			tool       	"VC++"
			name       	"GenerateIncludes"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"ApplyPattern"
			value      	FALSE)
		    (object Attribute
			tool       	"VC++"
			name       	"CreateBackupFiles"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"SupportCodeName"
			value      	FALSE)
		    (object Attribute
			tool       	"VC++"
			name       	"DocRevEngineer"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"CreateOverviewDiagrams"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"UpdateModelIDsInCode"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"AttributeTypes"
			value      	(value Text 
|attr1=bool
|attr2=short
|attr3=int
|attr4=long
|attr5=char
|attr6=float
|attr7=double
|attr8=void
|attr9=clock_t
|attr10=_complex
|attr11=_dev_t
|attr12=div_t
|attr13=_exception
|attr14=FILE
|attr15=_finddata_t
|attr16=_FPIEEE_RECORD
|attr17=fpos_t
|attr18=_HEAPINFO
|attr19=jmp_buf
|attr20=lconv
|attr21=ldiv_t
|attr22=_off_t
|attr23=_onexit_t
|attr24=_PNH
|attr25=ptrdiff_t
|attr26=sig_atomic_t
|attr27=size_t
|attr28=_stat
|attr29=time_t
|attr30=_timeb
|attr31=tm
|attr32=_utimbuf
|attr33=va_list
|attr34=wchar_t
|attr35=wctrans_t
|attr36=wctype_t
|attr37=_wfinddata_t
|attr38=_wfinddatai64_t
|attr39=wint_t
|attr40=ABORTPROC
|attr41=ACMDRIVERENUMCB
|attr42=ACMDRIVERPROC
|attr43=ACMFILTERCHOOSEHOOKPROC
|attr44=ACMFILTERENUMCB
|attr45=ACMFILTERTAGENUMCB
|attr46=ACMFORMATCHOOSEHOOKPROC
|attr47=ACMFORMATENUMCB
|attr48=ACMFORMATTAGENUMCB
|attr49=APPLET_PROC
|attr50=ATOM
|attr51=BOOL
|attr52=BOOLEAN
|attr53=BYTE
|attr54=CALINFO_ENUMPROC
|attr55=CALLBACK
|attr56=CHAR
|attr57=COLORREF
|attr58=CONST
|attr59=CRITICAL_SECTION
|attr60=CTRYID
|attr61=DATEFMT_ENUMPROC
|attr62=DESKTOPENUMPROC
|attr63=DLGPROC
|attr64=DRAWSTATEPROC
|attr65=DWORD
|attr66=EDITWORDBREAKPROC
|attr67=ENHMFENUMPROC
|attr68=ENUMRESLANGPROC
|attr69=ENUMRESNAMEPROC
|attr70=ENUMRESTYPEPROC
|attr71=FARPROC
|attr72=FILE_SEGMENT_ELEMENT
|attr73=FLOAT
|attr74=FONTENUMPROC
|attr75=GOBJENUMPROC
|attr76=GRAYSTRINGPROC
|attr77=HACCEL
|attr78=HANDLE
|attr79=HBITMAP
|attr80=HBRUSH
|attr81=HCOLORSPACE
|attr82=HCONV
|attr83=HCONVLIST
|attr84=HCURSOR
|attr85=HDC
|attr86=HDDEDATA
|attr87=HDESK
|attr88=HDROP
|attr89=HDWP
|attr90=HENHMETAFILE
|attr91=HFILE
|attr92=HFONT
|attr93=HGDIOBJ
|attr94=HGLOBAL
|attr95=HHOOK
|attr96=HICON
|attr97=HIMAGELIST
|attr98=HIMC
|attr99=HINSTANCE
|attr100=HKEY
|attr101=HKL
|attr102=HLOCAL
|attr103=HMENU
|attr104=HMETAFILE
|attr105=HMODULE
|attr106=HMONITOR
|attr107=HOOKPROC
|attr108=HPALETTE
|attr109=HPEN
|attr110=HRGN
|attr111=HRSRC
|attr112=HSZ
|attr113=HTREEITEM
|attr114=HWINSTA
|attr115=HWND
|attr116=INT
|attr117=IPADDR
|attr118=LANGID
|attr119=LCID
|attr120=LCSCSTYPE
|attr121=LCSGAMUTMATCH
|attr122=LCTYPE
|attr123=LINEDDAPROC
|attr124=LOCALE_ENUMPROC
|attr125=LONG
|attr126=LONGLONG
|attr127=LPARAM
|attr128=LPBOOL
|attr129=LPBYTE
|attr130=LPCCHOOKPROC
|attr131=LPCFHOOKPROC
|attr132=LPCOLORREF
|attr133=LPCRITICAL_SECTION
|attr134=LPCSTR
|attr135=LPCTSTR
|attr136=LPCVOID
|attr137=LPCWSTR
|attr138=LPDWORD
|attr139=LPFIBER_START_ROUTINE
|attr140=LPFRHOOKPROC
|attr141=LPHANDLE
|attr142=LPHANDLER_FUNCTION
|attr143=LPINT
|attr144=LPLONG
|attr145=LPOFNHOOKPROC
|attr146=LPPAGEPAINTHOOK
|attr147=LPPAGESETUPHOOK
|attr148=LPPRINTHOOKPROC
|attr149=LPPROGRESS_ROUTINE
|attr150=LPSETUPHOOKPROC
|attr151=LPSTR
|attr152=LPSTREAM
|attr153=LPTHREAD_START_ROUTINE
|attr154=LPTSTR
|attr155=LPVOID
|attr156=LPWORD
|attr157=LPWSTR
|attr158=LRESULT
|attr159=LUID
|attr160=PBOOL
|attr161=PBOOLEAN
|attr162=PBYTE
|attr163=PCHAR
|attr164=PCRITICAL_SECTION
|attr165=PCSTR
|attr166=PCTSTR
|attr167=PCWCH
|attr168=PCWSTR
|attr169=PDWORD
|attr170=PFLOAT
|attr171=PFNCALLBACK
|attr172=PHANDLE
|attr173=PHANDLER_ROUTINE
|attr174=PHKEY
|attr175=PINT
|attr176=PLCID
|attr177=PLONG
|attr178=PLUID
|attr179=PROPENUMPROC
|attr180=PROPENUMPROCEX
|attr181=PSHORT
|attr182=PSTR
|attr183=PTBYTE
|attr184=PTCHAR
|attr185=PTIMERAPCROUTINE
|attr186=PTSTR
|attr187=PUCHAR
|attr188=PUINT
|attr189=PULONG
|attr190=PUSHORT
|attr191=PVOID
|attr192=PWCHAR
|attr193=PWORD
|attr194=PWSTR
|attr195=REGISTERWORDENUMPROC
|attr196=REGSAM
|attr197=SC_HANDLE
|attr198=SC_LOCK
|attr199=SENDASYNCPROC
|attr200=SERVICE_STATUS_HANDLE
|attr201=SHORT
|attr202=TBYTE
|attr203=TCHAR
|attr204=TIMEFMT_ENUMPROC
|attr205=TIMERPROC
|attr206=UCHAR
|attr207=UINT
|attr208=ULONG
|attr209=ULONGLONG
|attr210=UNSIGNED
|attr211=USHORT
|attr212=VOID
|attr213=WCHAR
|attr214=WINAPI
|attr215=WINSTAENUMPROC
|attr216=WNDENUMPROC
|attr217=WNDPROC
|attr218=WORD
|attr219=WPARAM
|attr220=YIELDPROC
|attr221=CPoint
|attr222=CRect
|attr223=CSize
|attr224=CString
|attr225=CTime
|attr226=CTimeSpan
|attr227=CCreateContext
|attr228=CMemoryState
|attr229=COleSafeArray
|attr230=CPrintInfo
|attr231=HRESULT
			))
		    (object Attribute
			tool       	"VC++"
			name       	"Containers"
			value      	(value Text 
|cont1=CArray<$TYPE, $TYPE&>
|cont2=CByteArray
|cont3=CDWordArray
|cont4=CObArray
|cont5=CPtrArray
|cont6=CStringArray
|cont7=CUIntArray
|cont8=CWordArray
|cont9=CList<$TYPE, $TYPE&>
|cont10=CPtrList
|cont11=CObList
|cont12=CStringList
|cont13=CMapWordToPtr
|cont14=CMapPtrToWord
|cont15=CMapPtrToPtr
|cont16=CMapWordToOb
|cont17=CMapStringToPtr
|cont18=CMapStringToOb
|cont19=CMapStringToString
|cont20=CTypedPtrArray<CPtrArray, $TYPE*>
|cont21=CTypedPtrArray<CObArray, $TYPE*>
|cont22=CTypedPtrList<CObList, $TYPE*>
|cont23=CTypedPtrList<CPtrList, $TYPE*>
|cont24=CComObject<$TYPE>
|cont25=CComPtr<$TYPE>
|cont26=CComQIPtr<$TYPE>
|cont27=CComQIPtr<$TYPE, IID*>
			))
		    (object Attribute
			tool       	"VC++"
			name       	"ClassMethods"
			value      	(value Text 
|*_body=// ToDo: Add your specialized code here and/or call the base class
|cm1=$NAME()
|cm2=$NAME(orig:const $NAME&)
|cm3=<<virtual>> ~$NAME()
|cm4=operator=(rhs:$NAME&):$NAME&
|cm4_body=// ToDo: Add your specialized code here and/or call the base class||return rhs;
|cm5=<<const>> operator==(rhs:const $NAME&):bool
|cm5_body=// ToDo: Add your specialized code here and/or call the base class||return false;
|cm6=<<const>> operator!=(rhs:$NAME&):bool
|cm6_body=// ToDo: Add your specialized code here and/or call the base class||return false;
|cm7=<<const>> operator<(rhs:$NAME&):bool
|cm7_body=// ToDo: Add your specialized code here and/or call the base class||return false;
|cm8=<<const>> operator>(rhs:$NAME&):bool
|cm8_body=// ToDo: Add your specialized code here and/or call the base class||return false;
|cm9=<<const>> operator<=(rhs:$NAME&):bool
|cm9_body=// ToDo: Add your specialized code here and/or call the base class||return false;
|cm10=<<const>> operator>=(rhs:$NAME&):bool
|cm10_body=// ToDo: Add your specialized code here and/or call the base class||return false;
|cm11=<<friend>> operator>>(i:istream&, rhs:$NAME&):istream&
|cm11_body=// ToDo: Add your specialized code here and/or call the base class||return i;
|cm12=<<friend>> operator<<(o:ostream&, rhs:const $NAME&):ostream&
|cm12_body=// ToDo: Add your specialized code here and/or call the base class||return o;
			))
		    (object Attribute
			tool       	"VC++"
			name       	"Accessors"
			value      	(value Text 
|agf=<<const>> get_$BASICNAME():const $TYPE
|agf_body=return $NAME;
|asf=set_$BASICNAME(value:$TYPE):void
|asf_body=$NAME = value;|return;
|agv=<<const>> get_$BASICNAME():const $TYPE&
|agv_body=return $NAME;
|asv=set_$BASICNAME(value:$TYPE&):void
|asv_body=$NAME = value;|return;
|agp=<<const>> get_$BASICNAME():const $TYPE
|agp_body=return $NAME;
|asp=set_$BASICNAME(value:$TYPE):void
|asp_body=$NAME = value;|return;
|agr=<<const>> get_$BASICNAME():const $TYPE
|agr_body=return $NAME;
|asr=set_$BASICNAME(value:$TYPE):void
|asr_body=$NAME = value;|return;
|aga=<<const>> get_$BASICNAME(index:int):const $TYPE
|aga_body=return $NAME[index];
|asa=set_$BASICNAME(index:int, value:$TYPE):void
|asa_body=$NAME[index] = value;|return;
			))
		    (object Attribute
			tool       	"VC++"
			name       	"Conditionals"
			value      	(value Text 
|*_decl=#ifdef _DEBUG
|*_base=CObject
|cond1=<<virtual, const>> AssertValid():void
|cond1_body=$SUPERNAME::AssertValid();
|cond2=<<virtual, const>> Dump(dc:CDumpContext&):void
|cond2_body=$SUPERNAME::Dump(dc);
			))
		    (object Attribute
			tool       	"VC++"
			name       	"Patterns"
			value      	(value Text 
|patrn1=cm1,cm3,cond1,cond2
|Patrn1_name=Default
			))
		    (object Attribute
			tool       	"VC++"
			name       	"AtlClassPrefix"
			value      	"C")
		    (object Attribute
			tool       	"VC++"
			name       	"AtlInterfacePrefix"
			value      	"I")
		    (object Attribute
			tool       	"VC++"
			name       	"AtlTypeDescription"
			value      	"Class")
		    (object Attribute
			tool       	"VC++"
			name       	"DefaultLogicalPackage"
			value      	"$language Reverse Engineered/$component")
		    (object Attribute
			tool       	"VC++"
			name       	"DefaultComponentPackage"
			value      	"")))
	    (object Attribute
		tool       	"VC++"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"VC++"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"HeaderFileName"
			value      	"")
		    (object Attribute
			tool       	"VC++"
			name       	"CodeFileName"
			value      	"")))
	    (object Attribute
		tool       	"VC++"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"VC++"
			name       	"InternalMap"
			value      	(value Text 
|*:AUTO:AUTO
|
			))
		    (object Attribute
			tool       	"VC++"
			name       	"ExportMap"
			value      	(value Text 
|*:AUTO:AUTO
|
			))
		    (object Attribute
			tool       	"VC++"
			name       	"InitialSourceIncludes"
			value      	(value Text 
|"stdafx.h"
			))
		    (object Attribute
			tool       	"VC++"
			name       	"InitialHeaderIncludes"
			value      	(value Text ""))
		    (object Attribute
			tool       	"VC++"
			name       	"Copyright"
			value      	(value Text "Copyright (C) 1991 - 1999 Rational Software Corporation"))
		    (object Attribute
			tool       	"VC++"
			name       	"KindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"VC++"
				name       	"(none)"
				value      	300)
			    (object Attribute
				tool       	"VC++"
				name       	"DLL"
				value      	301)
			    (object Attribute
				tool       	"VC++"
				name       	"EXE"
				value      	302)
			    (object Attribute
				tool       	"VC++"
				name       	"MIDL"
				value      	303)))
		    (object Attribute
			tool       	"VC++"
			name       	"Kind"
			value      	("KindSet" 300))
		    (object Attribute
			tool       	"VC++"
			name       	"BodyExtensions"
			value      	(value Text 
|.cpp
|.cxx
|.inl
			))
		    (object Attribute
			tool       	"VC++"
			name       	"HeaderExtensions"
			value      	(value Text 
|.h
|.hpp
|.hxx
|inl
			))
		    (object Attribute
			tool       	"VC++"
			name       	"ProjectFolders"
			value      	(value Text 
|Source Files
|Header Files
			))
		    (object Attribute
			tool       	"VC++"
			name       	"UsePathMap"
			value      	FALSE)))
	    (object Attribute
		tool       	"VC++"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"VC++"
			name       	"Const"
			value      	FALSE)
		    (object Attribute
			tool       	"VC++"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"InitialValue"
			value      	"")))
	    (object Attribute
		tool       	"VC++"
		name       	"default__Uses"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"VC++"
			name       	"Generate"
			value      	TRUE)))
	    (object Attribute
		tool       	"VC++"
		name       	"default__Category"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"VC++"
			name       	"IsDirectory"
			value      	FALSE)
		    (object Attribute
			tool       	"VC++"
			name       	"Directory"
			value      	"")))
	    (object Attribute
		tool       	"VC++"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"VC++"
			name       	"Generate"
			value      	TRUE)))
	    (object Attribute
		tool       	"VC++"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"VC++"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"VC++"
			name       	"Inline"
			value      	FALSE)
		    (object Attribute
			tool       	"VC++"
			name       	"DefaultBody"
			value      	(value Text ""))))
	    (object Attribute
		tool       	"VC++"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"VisualStudio"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Web Modeler"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"XML_DTD"
		name       	"propertyId"
		value      	"809135966")
	    (object Attribute
		tool       	"XML_DTD"
		name       	"default__Project"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"XML_DTD"
			name       	"CreateMissingDirectories"
			value      	TRUE)
		    (object Attribute
			tool       	"XML_DTD"
			name       	"Editor"
			value      	("EditorType" 100))
		    (object Attribute
			tool       	"XML_DTD"
			name       	"StopOnError"
			value      	TRUE)
		    (object Attribute
			tool       	"XML_DTD"
			name       	"EditorType"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"XML_DTD"
				name       	"BuiltIn"
				value      	100)
			    (object Attribute
				tool       	"XML_DTD"
				name       	"WindowsShell"
				value      	101)))))
	    (object Attribute
		tool       	"XML_DTD"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"XML_DTD"
			name       	"Entity_SystemID"
			value      	"")
		    (object Attribute
			tool       	"XML_DTD"
			name       	"Entity_PublicID"
			value      	"")
		    (object Attribute
			tool       	"XML_DTD"
			name       	"NotationValue"
			value      	"")
		    (object Attribute
			tool       	"XML_DTD"
			name       	"InternalValue"
			value      	"")
		    (object Attribute
			tool       	"XML_DTD"
			name       	"ParameterEntity"
			value      	FALSE)
		    (object Attribute
			tool       	"XML_DTD"
			name       	"ExternalEntity"
			value      	FALSE)
		    (object Attribute
			tool       	"XML_DTD"
			name       	"Notation_SystemID"
			value      	"")
		    (object Attribute
			tool       	"XML_DTD"
			name       	"Notation_PublicID"
			value      	"")))
	    (object Attribute
		tool       	"XML_DTD"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"XML_DTD"
			name       	"DefaultDeclType"
			value      	"")))
	    (object Attribute
		tool       	"XML_DTD"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"XML_DTD"
			name       	"Assign All"
			value      	FALSE)
		    (object Attribute
			tool       	"XML_DTD"
			name       	"ComponentPath"
			value      	"")))
	    (object Attribute
		tool       	"XML_DTD"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Cplusplus"
		name       	"propertyId"
		value      	"809135966")
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Synchronize"
			value      	TRUE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"InitialValue"
			value      	"")))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Inherit"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Synchronize"
			value      	TRUE)))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Synchronize"
			value      	TRUE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"RevEngRootDirectory"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"RootPackage"
			value      	"C++ Reverse Engineered")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"RevEngDirectoriesAsPackages"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"HeaderFileExtension"
			value      	".h")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ImplementationFileExtension"
			value      	".cpp")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"NewHeaderFileDirectory"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"NewImplementationFileDirectory"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"FileCapitalization"
			value      	("FileCapitalizationSet" 0))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeGenExtraDirectories"
			value      	("CodeGenExtraDirectoriesSet" 0))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"StripClassPrefix"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"UseTabs"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"TabWidth"
			value      	8)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"IndentWidth"
			value      	4)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"AccessIndentation"
			value      	-2)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CreateBackupFiles"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ModelIdCommentRules"
			value      	("ModelIdCommentRulesSet" 1))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CommentRules"
			value      	("CommentRulesSet" 1))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"PageWidth"
			value      	80)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ClassMemberOrder"
			value      	("MemberOrderSet" 1))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"OneParameterPerLine"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"NamespaceBraceStyle"
			value      	("BraceStyleSet" 2))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ClassBraceStyle"
			value      	("BraceStyleSet" 2))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"FunctionBraceStyle"
			value      	("BraceStyleSet" 2))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Copyright"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"InitialHeaderIncludes"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"InitialBodyIncludes"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeGenExtraDirectoriesSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"None"
				value      	0)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Namespaces"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Packages"
				value      	2)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"FileCapitalizationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Same as model"
				value      	0)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Lower case"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Upper case"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Lower case with underscores"
				value      	3)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"BraceStyleSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B1"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B2"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B3"
				value      	3)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B4"
				value      	4)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B5"
				value      	5)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"MemberOrderSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Public First"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Private First"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Order by kind"
				value      	3)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Unordered"
				value      	4)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ModelIdCommentRulesSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Code generation only"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Code generation and reverse engineering"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Never generate model IDs"
				value      	3)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CommentRulesSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Always synchronize"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Code generation only"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Reverse engineering only"
				value      	3)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Never synchronize"
				value      	4)))))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Module-Body"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Synchronize"
			value      	TRUE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"RevEngRootDirectory"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"RootPackage"
			value      	"C++ Reverse Engineered")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"RevEngDirectoriesAsPackages"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"HeaderFileExtension"
			value      	".h")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ImplementationFileExtension"
			value      	".cpp")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"NewHeaderFileDirectory"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"NewImplementationFileDirectory"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"FileCapitalization"
			value      	("FileCapitalizationSet" 0))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeGenExtraDirectories"
			value      	("CodeGenExtraDirectoriesSet" 0))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"StripClassPrefix"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"UseTabs"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"TabWidth"
			value      	8)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"IndentWidth"
			value      	4)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"AccessIndentation"
			value      	-2)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CreateBackupFiles"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ModelIdCommentRules"
			value      	("ModelIdCommentRulesSet" 1))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CommentRules"
			value      	("CommentRulesSet" 1))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"PageWidth"
			value      	80)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ClassMemberOrder"
			value      	("MemberOrderSet" 1))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"OneParameterPerLine"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"NamespaceBraceStyle"
			value      	("BraceStyleSet" 2))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ClassBraceStyle"
			value      	("BraceStyleSet" 2))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"FunctionBraceStyle"
			value      	("BraceStyleSet" 2))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Copyright"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"InitialHeaderIncludes"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"InitialBodyIncludes"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeGenExtraDirectoriesSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"None"
				value      	0)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Namespaces"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Packages"
				value      	2)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"FileCapitalizationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Same as model"
				value      	0)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Lower case"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Upper case"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Lower case with underscores"
				value      	3)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"BraceStyleSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B1"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B2"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B3"
				value      	3)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B4"
				value      	4)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"B5"
				value      	5)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"MemberOrderSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Public First"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Private First"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Order by kind"
				value      	3)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Unordered"
				value      	4)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ModelIdCommentRulesSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Code generation only"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Code generation and reverse engineering"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Never generate model IDs"
				value      	3)))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CommentRulesSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Always synchronize"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Code generation only"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Reverse engineering only"
				value      	3)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Never synchronize"
				value      	4)))))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Param"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeName"
			value      	"")))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Synchronize"
			value      	TRUE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeName"
			value      	"")))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Synchronize"
			value      	TRUE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"InitialCodeBody"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Inline"
			value      	FALSE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"GenerateFunctionBody"
			value      	("GenerateFunctionBodySet" 2))
		    (object Attribute
			tool       	"Cplusplus"
			name       	"GenerateFunctionBodySet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Cplusplus"
				name       	"Default"
				value      	2)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"True"
				value      	1)
			    (object Attribute
				tool       	"Cplusplus"
				name       	"False"
				value      	0)))))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"Synchronize"
			value      	TRUE)
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"ImplementationType"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"HeaderSourceFile"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"BodySourceFile"
			value      	"")))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Category"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Cplusplus"
			name       	"IsNamespace"
			value      	FALSE)))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"default__Uses"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Cplusplus"
			name       	"BodyReferenceOnly"
			value      	FALSE)))
	    (object Attribute
		tool       	"Cplusplus"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"ANSIConvert"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Ada83"
		name       	"propertyId"
		value      	"838326200")
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Project"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"SpecFileExtension"
			value      	"1.ada")
		    (object Attribute
			tool       	"Ada83"
			name       	"SpecFileBackupExtension"
			value      	"1.ad~")
		    (object Attribute
			tool       	"Ada83"
			name       	"SpecFileTemporaryExtension"
			value      	"1.ad#")
		    (object Attribute
			tool       	"Ada83"
			name       	"BodyFileExtension"
			value      	"2.ada")
		    (object Attribute
			tool       	"Ada83"
			name       	"BodyFileBackupExtension"
			value      	"2.ad~")
		    (object Attribute
			tool       	"Ada83"
			name       	"BodyFileTemporaryExtension"
			value      	"2.ad#")
		    (object Attribute
			tool       	"Ada83"
			name       	"CreateMissingDirectories"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"GenerateBodies"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"GenerateAccessorOperations"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"GenerateStandardOperations"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"DefaultCodeBody"
			value      	"[statement]")
		    (object Attribute
			tool       	"Ada83"
			name       	"ImplicitParameter"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"CommentWidth"
			value      	60)
		    (object Attribute
			tool       	"Ada83"
			name       	"StopOnError"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"ErrorLimit"
			value      	30)
		    (object Attribute
			tool       	"Ada83"
			name       	"UseFileName"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"Directory"
			value      	"$ROSEADA83_SOURCE")))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"ClassName"
			value      	"Object")
		    (object Attribute
			tool       	"Ada83"
			name       	"ClassAccess"
			value      	("ImplementationSet" 43))
		    (object Attribute
			tool       	"Ada83"
			name       	"ImplementationType"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"IsSubtype"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"PolymorphicUnit"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"HandleName"
			value      	"Handle")
		    (object Attribute
			tool       	"Ada83"
			name       	"HandleAccess"
			value      	("ImplementationSet" 45))
		    (object Attribute
			tool       	"Ada83"
			name       	"Discriminant"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"Variant"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"EnumerationLiteralPrefix"
			value      	"A_")
		    (object Attribute
			tool       	"Ada83"
			name       	"RecordFieldPrefix"
			value      	"The_")
		    (object Attribute
			tool       	"Ada83"
			name       	"GenerateAccessorOperations"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"GenerateStandardOperations"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"ImplicitParameter"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"ClassParameterName"
			value      	"This")
		    (object Attribute
			tool       	"Ada83"
			name       	"DefaultConstructorKind"
			value      	("ConstructorKindSet" 199))
		    (object Attribute
			tool       	"Ada83"
			name       	"DefaultConstructorName"
			value      	"Create")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineDefaultConstructor"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"CopyConstructorKind"
			value      	("ConstructorKindSet" 199))
		    (object Attribute
			tool       	"Ada83"
			name       	"CopyConstructorName"
			value      	"Copy")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineCopyConstructor"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"DestructorName"
			value      	"Free")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineDestructor"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"ClassEqualityOperation"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"HandleEqualityOperation"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineEquality"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"IsTask"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"Representation"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"ImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Public"
				value      	45)
			    (object Attribute
				tool       	"Ada83"
				name       	"Private"
				value      	43)
			    (object Attribute
				tool       	"Ada83"
				name       	"LimitedPrivate"
				value      	200)
			    (object Attribute
				tool       	"Ada83"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada83"
			name       	"ConstructorKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada83"
				name       	"Function"
				value      	199)
			    (object Attribute
				tool       	"Ada83"
				name       	"DoNotCreate"
				value      	201)))))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"CopyrightNotice"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"FileName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"ReturnType"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"GenericFormalParameters"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"AdditionalWiths"
			value      	(value Text ""))))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Module-Body"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"CopyrightNotice"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"FileName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"ReturnType"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"AdditionalWiths"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"IsSubunit"
			value      	FALSE)))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"SubprogramImplementation"
			value      	("SubprogramImplementationSet" 2))
		    (object Attribute
			tool       	"Ada83"
			name       	"Renames"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"ClassParameterMode"
			value      	("ParameterModeSet" 203))
		    (object Attribute
			tool       	"Ada83"
			name       	"Inline"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"EntryCode"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"ExitCode"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"InitialCodeBody"
			value      	"${default}")
		    (object Attribute
			tool       	"Ada83"
			name       	"Representation"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"SubprogramImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Spec"
				value      	224)
			    (object Attribute
				tool       	"Ada83"
				name       	"Body"
				value      	2)
			    (object Attribute
				tool       	"Ada83"
				name       	"Renaming"
				value      	222)
			    (object Attribute
				tool       	"Ada83"
				name       	"Separate"
				value      	223)))
		    (object Attribute
			tool       	"Ada83"
			name       	"ParameterModeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Default"
				value      	232)
			    (object Attribute
				tool       	"Ada83"
				name       	"In"
				value      	204)
			    (object Attribute
				tool       	"Ada83"
				name       	"Out"
				value      	205)
			    (object Attribute
				tool       	"Ada83"
				name       	"InOut"
				value      	203)
			    (object Attribute
				tool       	"Ada83"
				name       	"FunctionReturn"
				value      	206)
			    (object Attribute
				tool       	"Ada83"
				name       	"DoNotCreate"
				value      	201)))))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Param"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"Mode"
			value      	("ParameterModeSet" 232))
		    (object Attribute
			tool       	"Ada83"
			name       	"ParameterModeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Default"
				value      	232)
			    (object Attribute
				tool       	"Ada83"
				name       	"In"
				value      	204)
			    (object Attribute
				tool       	"Ada83"
				name       	"Out"
				value      	205)
			    (object Attribute
				tool       	"Ada83"
				name       	"InOut"
				value      	203)))))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Has"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"NameIfUnlabeled"
			value      	"The_${supplier}")
		    (object Attribute
			tool       	"Ada83"
			name       	"DataMemberName"
			value      	"${relationship}")
		    (object Attribute
			tool       	"Ada83"
			name       	"GetName"
			value      	"Get_${relationship}")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineGet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"SetName"
			value      	"Set_${relationship}")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineSet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"IsConstant"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"InitialValue"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"Declare"
			value      	("DeclareSet" 234))
		    (object Attribute
			tool       	"Ada83"
			name       	"Variant"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"ContainerGeneric"
			value      	"List")
		    (object Attribute
			tool       	"Ada83"
			name       	"ContainerType"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"ContainerDeclarations"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"SelectorName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"SelectorType"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"DeclareSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Before"
				value      	233)
			    (object Attribute
				tool       	"Ada83"
				name       	"After"
				value      	234)))))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"DataMemberName"
			value      	"${attribute}")
		    (object Attribute
			tool       	"Ada83"
			name       	"GetName"
			value      	"Get_${attribute}")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineGet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"SetName"
			value      	"Set_${attribute}")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineSet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"IsConstant"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"InitialValue"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"Declare"
			value      	("DeclareSet" 234))
		    (object Attribute
			tool       	"Ada83"
			name       	"Variant"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"Representation"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"DeclareSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Before"
				value      	233)
			    (object Attribute
				tool       	"Ada83"
				name       	"After"
				value      	234)))))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Association"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"NameIfUnlabeled"
			value      	"The_${targetClass}")
		    (object Attribute
			tool       	"Ada83"
			name       	"GetName"
			value      	"Get_${association}")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineGet"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"SetName"
			value      	"Set_${association}")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineSet"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"GenerateAssociate"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada83"
			name       	"AssociateName"
			value      	"Associate")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineAssociate"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"GenerateDissociate"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada83"
			name       	"DissociateName"
			value      	"Dissociate")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineDissociate"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"ProcedureKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada83"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada83"
			name       	"FunctionKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Function"
				value      	199)
			    (object Attribute
				tool       	"Ada83"
				name       	"DoNotCreate"
				value      	201)))))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"NameIfUnlabeled"
			value      	"The_${targetClass}")
		    (object Attribute
			tool       	"Ada83"
			name       	"DataMemberName"
			value      	"${target}")
		    (object Attribute
			tool       	"Ada83"
			name       	"GetName"
			value      	"Get_${target}")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineGet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"SetName"
			value      	"Set_${target}")
		    (object Attribute
			tool       	"Ada83"
			name       	"InlineSet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada83"
			name       	"IsConstant"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada83"
			name       	"InitialValue"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"Declare"
			value      	("DeclareSet" 234))
		    (object Attribute
			tool       	"Ada83"
			name       	"Representation"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"ContainerGeneric"
			value      	"List")
		    (object Attribute
			tool       	"Ada83"
			name       	"ContainerType"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"ContainerDeclarations"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada83"
			name       	"SelectorName"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"SelectorType"
			value      	"")
		    (object Attribute
			tool       	"Ada83"
			name       	"ProcedureKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada83"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada83"
			name       	"DeclareSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada83"
				name       	"Before"
				value      	233)
			    (object Attribute
				tool       	"Ada83"
				name       	"After"
				value      	234)))))
	    (object Attribute
		tool       	"Ada83"
		name       	"default__Subsystem"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada83"
			name       	"Directory"
			value      	"AUTO GENERATE")))
	    (object Attribute
		tool       	"Ada83"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Ada95"
		name       	"propertyId"
		value      	"838326200")
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Project"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"SpecFileExtension"
			value      	"1.ada")
		    (object Attribute
			tool       	"Ada95"
			name       	"SpecFileBackupExtension"
			value      	"1.ad~")
		    (object Attribute
			tool       	"Ada95"
			name       	"SpecFileTemporaryExtension"
			value      	"1.ad#")
		    (object Attribute
			tool       	"Ada95"
			name       	"BodyFileExtension"
			value      	"2.ada")
		    (object Attribute
			tool       	"Ada95"
			name       	"BodyFileBackupExtension"
			value      	"2.ad~")
		    (object Attribute
			tool       	"Ada95"
			name       	"BodyFileTemporaryExtension"
			value      	"2.ad#")
		    (object Attribute
			tool       	"Ada95"
			name       	"CreateMissingDirectories"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"UseColonNotation"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateBodies"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessorOperations"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateStandardOperations"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"DefaultCodeBody"
			value      	"[statement]")
		    (object Attribute
			tool       	"Ada95"
			name       	"ImplicitParameter"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"CommentWidth"
			value      	60)
		    (object Attribute
			tool       	"Ada95"
			name       	"StopOnError"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"ErrorLimit"
			value      	30)
		    (object Attribute
			tool       	"Ada95"
			name       	"UseFileName"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"Directory"
			value      	"$ROSEADA95_SOURCE")))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeName"
			value      	"Object")
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeVisibility"
			value      	("TypeVisibilitySet" 43))
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeImplementation"
			value      	("TypeImplementationSet" 208))
		    (object Attribute
			tool       	"Ada95"
			name       	"IncompleteType"
			value      	("IncompleteTypeSet" 1))
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeControl"
			value      	("TypeControlSet" 225))
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeControlName"
			value      	"Controlled_${type}")
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeControlVisibility"
			value      	("TypeVisibilitySet" 43))
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeDefinition"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordImplementation"
			value      	("RecordImplementationSet" 209))
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordKindPackageName"
			value      	"${class}_Record_Kinds")
		    (object Attribute
			tool       	"Ada95"
			name       	"IsLimited"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"IsSubtype"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessType"
			value      	("GenerateAccessTypeSet" 230))
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessTypeName"
			value      	"Handle")
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessTypeVisibility"
			value      	("TypeVisibilitySet" 45))
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessTypeDefinition"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessClassWide"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"MaybeAliased"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"ParameterizedImplementation"
			value      	("ParameterizedImplementationSet" 11))
		    (object Attribute
			tool       	"Ada95"
			name       	"ParentClassName"
			value      	"Superclass")
		    (object Attribute
			tool       	"Ada95"
			name       	"EnumerationLiteralPrefix"
			value      	"A_")
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldPrefix"
			value      	"The_")
		    (object Attribute
			tool       	"Ada95"
			name       	"ArrayOfTypeName"
			value      	"Array_Of_${type}")
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessArrayOfTypeName"
			value      	"Access_Array_Of_${type}")
		    (object Attribute
			tool       	"Ada95"
			name       	"ArrayOfAccessTypeName"
			value      	"Array_Of_${access_type}")
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessArrayOfAccessTypeName"
			value      	"Access_Array_Of_${access_type}")
		    (object Attribute
			tool       	"Ada95"
			name       	"ArrayIndexDefinition"
			value      	"Positive range <>")
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessorOperations"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateStandardOperations"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"ImplicitParameter"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"ImplicitParameterName"
			value      	"This")
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateDefaultConstructor"
			value      	("SubprogramKindSet" 199))
		    (object Attribute
			tool       	"Ada95"
			name       	"DefaultConstructorName"
			value      	"Create")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineDefaultConstructor"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateCopyConstructor"
			value      	("SubprogramKindSet" 199))
		    (object Attribute
			tool       	"Ada95"
			name       	"CopyConstructorName"
			value      	"Copy")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineCopyConstructor"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateDestructor"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada95"
			name       	"DestructorName"
			value      	"Free")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineDestructor"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateTypeEquality"
			value      	("FunctionKindSet" 201))
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeEqualityName"
			value      	
|"="
			)
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineEquality"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"Representation"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Tagged"
				value      	208)
			    (object Attribute
				tool       	"Ada95"
				name       	"Record"
				value      	210)
			    (object Attribute
				tool       	"Ada95"
				name       	"Mixin"
				value      	211)
			    (object Attribute
				tool       	"Ada95"
				name       	"Protected"
				value      	44)
			    (object Attribute
				tool       	"Ada95"
				name       	"Task"
				value      	212)))
		    (object Attribute
			tool       	"Ada95"
			name       	"IncompleteTypeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotDeclare"
				value      	1)
			    (object Attribute
				tool       	"Ada95"
				name       	"NoDiscriminantPart"
				value      	2)
			    (object Attribute
				tool       	"Ada95"
				name       	"UnknownDiscriminantPart"
				value      	3)
			    (object Attribute
				tool       	"Ada95"
				name       	"KnownDiscriminantPart"
				value      	4)))
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"SingleType"
				value      	209)
			    (object Attribute
				tool       	"Ada95"
				name       	"MultipleTypes"
				value      	213)))
		    (object Attribute
			tool       	"Ada95"
			name       	"ParameterizedImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Generic"
				value      	11)
			    (object Attribute
				tool       	"Ada95"
				name       	"Unconstrained"
				value      	214)))
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeVisibilitySet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Public"
				value      	45)
			    (object Attribute
				tool       	"Ada95"
				name       	"Private"
				value      	43)))
		    (object Attribute
			tool       	"Ada95"
			name       	"SubprogramKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada95"
				name       	"Function"
				value      	199)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada95"
			name       	"ProcedureKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada95"
			name       	"FunctionKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Function"
				value      	199)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada95"
			name       	"TypeControlSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"None"
				value      	225)
			    (object Attribute
				tool       	"Ada95"
				name       	"InitializationOnly"
				value      	226)
			    (object Attribute
				tool       	"Ada95"
				name       	"AssignmentFinalizationOnly"
				value      	227)
			    (object Attribute
				tool       	"Ada95"
				name       	"All"
				value      	228)))
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessTypeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Always"
				value      	229)
			    (object Attribute
				tool       	"Ada95"
				name       	"Auto"
				value      	230)))))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"CopyrightNotice"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"FileName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"ReturnType"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"GenericFormalParameters"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"AdditionalWiths"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"IsPrivate"
			value      	FALSE)))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Module-Body"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"Generate"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"CopyrightNotice"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"FileName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"ReturnType"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"AdditionalWiths"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"IsSubunit"
			value      	FALSE)))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"SubprogramImplementation"
			value      	("SubprogramImplementationSet" 2))
		    (object Attribute
			tool       	"Ada95"
			name       	"Renames"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateOverriding"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"ImplicitParameterMode"
			value      	("ParameterModeSet" 203))
		    (object Attribute
			tool       	"Ada95"
			name       	"ImplicitParameterClassWide"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessOperation"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"Inline"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"EntryCode"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"ExitCode"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"InitialCodeBody"
			value      	"${default}")
		    (object Attribute
			tool       	"Ada95"
			name       	"EntryBarrierCondition"
			value      	"True")
		    (object Attribute
			tool       	"Ada95"
			name       	"Representation"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"SubprogramImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Spec"
				value      	224)
			    (object Attribute
				tool       	"Ada95"
				name       	"Body"
				value      	2)
			    (object Attribute
				tool       	"Ada95"
				name       	"Abstract"
				value      	221)
			    (object Attribute
				tool       	"Ada95"
				name       	"Renaming"
				value      	222)
			    (object Attribute
				tool       	"Ada95"
				name       	"RenamingAsBody"
				value      	231)
			    (object Attribute
				tool       	"Ada95"
				name       	"Separate"
				value      	223)))
		    (object Attribute
			tool       	"Ada95"
			name       	"ParameterModeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Default"
				value      	232)
			    (object Attribute
				tool       	"Ada95"
				name       	"In"
				value      	204)
			    (object Attribute
				tool       	"Ada95"
				name       	"Out"
				value      	205)
			    (object Attribute
				tool       	"Ada95"
				name       	"InOut"
				value      	203)
			    (object Attribute
				tool       	"Ada95"
				name       	"Access"
				value      	220)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Param"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"Mode"
			value      	("ParameterModeSet" 232))
		    (object Attribute
			tool       	"Ada95"
			name       	"ParameterModeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Default"
				value      	232)
			    (object Attribute
				tool       	"Ada95"
				name       	"In"
				value      	204)
			    (object Attribute
				tool       	"Ada95"
				name       	"Out"
				value      	205)
			    (object Attribute
				tool       	"Ada95"
				name       	"InOut"
				value      	203)
			    (object Attribute
				tool       	"Ada95"
				name       	"Access"
				value      	220)))))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Has"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"NameIfUnlabeled"
			value      	"The_${supplier}")
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldImplementation"
			value      	("RecordFieldImplementationSet" 216))
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessDiscriminantClassWide"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldName"
			value      	"${relationship}")
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateGet"
			value      	("FunctionKindSet" 199))
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessGet"
			value      	("FunctionKindSet" 201))
		    (object Attribute
			tool       	"Ada95"
			name       	"GetName"
			value      	"Get_${relationship}")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineGet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateSet"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessSet"
			value      	("ProcedureKindSet" 201))
		    (object Attribute
			tool       	"Ada95"
			name       	"SetName"
			value      	"Set_${relationship}")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineSet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"IsAliased"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"IsConstant"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"InitialValue"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"Declare"
			value      	("DeclareSet" 234))
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerImplementation"
			value      	("ContainerImplementationSet" 217))
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerGeneric"
			value      	"List")
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerType"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerDeclarations"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"SelectorName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"SelectorType"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"DeclareSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Before"
				value      	233)
			    (object Attribute
				tool       	"Ada95"
				name       	"After"
				value      	234)))
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Component"
				value      	216)
			    (object Attribute
				tool       	"Ada95"
				name       	"Discriminant"
				value      	218)
			    (object Attribute
				tool       	"Ada95"
				name       	"AccessDiscriminant"
				value      	219)))
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Array"
				value      	217)
			    (object Attribute
				tool       	"Ada95"
				name       	"Generic"
				value      	11)))
		    (object Attribute
			tool       	"Ada95"
			name       	"ProcedureKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada95"
			name       	"FunctionKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Function"
				value      	199)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldImplementation"
			value      	("RecordFieldImplementationSet" 216))
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessDiscriminantClassWide"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldName"
			value      	"${attribute}")
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateGet"
			value      	("FunctionKindSet" 199))
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessGet"
			value      	("FunctionKindSet" 201))
		    (object Attribute
			tool       	"Ada95"
			name       	"GetName"
			value      	"Get_${attribute}")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineGet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateSet"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessSet"
			value      	("ProcedureKindSet" 201))
		    (object Attribute
			tool       	"Ada95"
			name       	"SetName"
			value      	"Set_${attribute}")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineSet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"IsAliased"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"IsConstant"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"InitialValue"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"Declare"
			value      	("DeclareSet" 234))
		    (object Attribute
			tool       	"Ada95"
			name       	"Representation"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"DeclareSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Before"
				value      	233)
			    (object Attribute
				tool       	"Ada95"
				name       	"After"
				value      	234)))
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Component"
				value      	216)
			    (object Attribute
				tool       	"Ada95"
				name       	"Discriminant"
				value      	218)
			    (object Attribute
				tool       	"Ada95"
				name       	"AccessDiscriminant"
				value      	219)))
		    (object Attribute
			tool       	"Ada95"
			name       	"ProcedureKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada95"
			name       	"FunctionKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Function"
				value      	199)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Association"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"NameIfUnlabeled"
			value      	"The_${targetClass}")
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateGet"
			value      	("FunctionKindSet" 199))
		    (object Attribute
			tool       	"Ada95"
			name       	"GetName"
			value      	"Get_${association}")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineGet"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateSet"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada95"
			name       	"SetName"
			value      	"Set_${association}")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineSet"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAssociate"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada95"
			name       	"AssociateName"
			value      	"Associate")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineAssociate"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateDissociate"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada95"
			name       	"DissociateName"
			value      	"Dissociate")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineDissociate"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"ProcedureKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada95"
			name       	"FunctionKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Function"
				value      	199)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"CodeName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"NameIfUnlabeled"
			value      	"The_${targetClass}")
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldImplementation"
			value      	("RecordFieldImplementationSet" 216))
		    (object Attribute
			tool       	"Ada95"
			name       	"AccessDiscriminantClassWide"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldName"
			value      	"${target}")
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateGet"
			value      	("FunctionKindSet" 199))
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessGet"
			value      	("FunctionKindSet" 201))
		    (object Attribute
			tool       	"Ada95"
			name       	"GetName"
			value      	"Get_${target}")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineGet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateSet"
			value      	("ProcedureKindSet" 202))
		    (object Attribute
			tool       	"Ada95"
			name       	"GenerateAccessSet"
			value      	("ProcedureKindSet" 201))
		    (object Attribute
			tool       	"Ada95"
			name       	"SetName"
			value      	"Set_${target}")
		    (object Attribute
			tool       	"Ada95"
			name       	"InlineSet"
			value      	TRUE)
		    (object Attribute
			tool       	"Ada95"
			name       	"IsAliased"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"IsConstant"
			value      	FALSE)
		    (object Attribute
			tool       	"Ada95"
			name       	"InitialValue"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"Declare"
			value      	("DeclareSet" 234))
		    (object Attribute
			tool       	"Ada95"
			name       	"Representation"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerImplementation"
			value      	("ContainerImplementationSet" 217))
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerGeneric"
			value      	"List")
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerType"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerDeclarations"
			value      	(value Text ""))
		    (object Attribute
			tool       	"Ada95"
			name       	"SelectorName"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"SelectorType"
			value      	"")
		    (object Attribute
			tool       	"Ada95"
			name       	"ProcedureKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Procedure"
				value      	202)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))
		    (object Attribute
			tool       	"Ada95"
			name       	"DeclareSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Before"
				value      	233)
			    (object Attribute
				tool       	"Ada95"
				name       	"After"
				value      	234)))
		    (object Attribute
			tool       	"Ada95"
			name       	"RecordFieldImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Component"
				value      	216)
			    (object Attribute
				tool       	"Ada95"
				name       	"Discriminant"
				value      	218)
			    (object Attribute
				tool       	"Ada95"
				name       	"AccessDiscriminant"
				value      	219)))
		    (object Attribute
			tool       	"Ada95"
			name       	"ContainerImplementationSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Array"
				value      	217)
			    (object Attribute
				tool       	"Ada95"
				name       	"Generic"
				value      	11)))
		    (object Attribute
			tool       	"Ada95"
			name       	"FunctionKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Ada95"
				name       	"Function"
				value      	199)
			    (object Attribute
				tool       	"Ada95"
				name       	"DoNotCreate"
				value      	201)))))
	    (object Attribute
		tool       	"Ada95"
		name       	"default__Subsystem"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Ada95"
			name       	"Directory"
			value      	"AUTO GENERATE")))
	    (object Attribute
		tool       	"Ada95"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"CORBA"
		name       	"default__Param"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"CORBA"
			name       	"Direction"
			value      	("ParamDirectionTypeSet" 102))
		    (object Attribute
			tool       	"CORBA"
			name       	"ParamDirectionTypeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"CORBA"
				name       	"in"
				value      	102)
			    (object Attribute
				tool       	"CORBA"
				name       	"inout"
				value      	103)
			    (object Attribute
				tool       	"CORBA"
				name       	"out"
				value      	104)))))
	    (object Attribute
		tool       	"Deploy"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Oracle8"
		name       	"propertyId"
		value      	"360000002")
	    (object Attribute
		tool       	"Oracle8"
		name       	"default__Project"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Oracle8"
			name       	"DDLScriptFilename"
			value      	"DDL1.SQL")
		    (object Attribute
			tool       	"Oracle8"
			name       	"DropClause"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"PrimaryKeyColumnName"
			value      	"_ID")
		    (object Attribute
			tool       	"Oracle8"
			name       	"PrimaryKeyColumnType"
			value      	"NUMBER(5,0)")
		    (object Attribute
			tool       	"Oracle8"
			name       	"SchemaNamePrefix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"SchemaNameSuffix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"TableNamePrefix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"TableNameSuffix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"TypeNamePrefix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"TypeNameSuffix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"ViewNamePrefix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"ViewNameSuffix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"VarrayNamePrefix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"VarrayNameSuffix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"NestedTableNamePrefix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"NestedTableNameSuffix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"ObjectTableNamePrefix"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"ObjectTableNameSuffix"
			value      	"")))
	    (object Attribute
		tool       	"Oracle8"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsSchema"
			value      	FALSE)))
	    (object Attribute
		tool       	"Oracle8"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Oracle8"
			name       	"OID"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"WhereClause"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"CheckConstraint"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"CollectionTypeLength"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"CollectionTypePrecision"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"CollectionTypeScale"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"CollectionOfREFS"
			value      	FALSE)))
	    (object Attribute
		tool       	"Oracle8"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Oracle8"
			name       	"MethodKind"
			value      	("MethodKindSet" 1903))
		    (object Attribute
			tool       	"Oracle8"
			name       	"OverloadID"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"OrderNumber"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsReadNoDataState"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsReadNoProcessState"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsWriteNoDataState"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsWriteNoProcessState"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsSelfish"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerType"
			value      	("TriggerTypeSet" 1801))
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerEvent"
			value      	("TriggerEventSet" 1601))
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerText"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerReferencingNames"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerForEach"
			value      	("TriggerForEachSet" 1701))
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerWhenClause"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"MethodKindSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Oracle8"
				name       	"MapMethod"
				value      	1901)
			    (object Attribute
				tool       	"Oracle8"
				name       	"OrderMethod"
				value      	1902)
			    (object Attribute
				tool       	"Oracle8"
				name       	"Function"
				value      	1903)
			    (object Attribute
				tool       	"Oracle8"
				name       	"Procedure"
				value      	1904)
			    (object Attribute
				tool       	"Oracle8"
				name       	"Operator"
				value      	1905)
			    (object Attribute
				tool       	"Oracle8"
				name       	"Constructor"
				value      	1906)
			    (object Attribute
				tool       	"Oracle8"
				name       	"Destructor"
				value      	1907)
			    (object Attribute
				tool       	"Oracle8"
				name       	"Trigger"
				value      	1908)
			    (object Attribute
				tool       	"Oracle8"
				name       	"Calculated"
				value      	1909)))
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerTypeSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Oracle8"
				name       	"AFTER"
				value      	1801)
			    (object Attribute
				tool       	"Oracle8"
				name       	"BEFORE"
				value      	1802)
			    (object Attribute
				tool       	"Oracle8"
				name       	"INSTEAD OF"
				value      	1803)))
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerForEachSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Oracle8"
				name       	"ROW"
				value      	1701)
			    (object Attribute
				tool       	"Oracle8"
				name       	"STATEMENT"
				value      	1702)))
		    (object Attribute
			tool       	"Oracle8"
			name       	"TriggerEventSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Oracle8"
				name       	"INSERT"
				value      	1601)
			    (object Attribute
				tool       	"Oracle8"
				name       	"UPDATE"
				value      	1602)
			    (object Attribute
				tool       	"Oracle8"
				name       	"DELETE"
				value      	1603)
			    (object Attribute
				tool       	"Oracle8"
				name       	"INSERT OR UPDATE"
				value      	1604)
			    (object Attribute
				tool       	"Oracle8"
				name       	"INSERT OR DELETE"
				value      	1605)
			    (object Attribute
				tool       	"Oracle8"
				name       	"UPDATE OR DELETE"
				value      	1606)
			    (object Attribute
				tool       	"Oracle8"
				name       	"INSERT OR UPDATE OR DELETE"
				value      	1607)))))
	    (object Attribute
		tool       	"Oracle8"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Oracle8"
			name       	"OrderNumber"
			value      	"")))
	    (object Attribute
		tool       	"Oracle8"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Oracle8"
			name       	"OrderNumber"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsUnique"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"NullsAllowed"
			value      	TRUE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"Length"
			value      	"")
		    (object Attribute
			tool       	"Oracle8"
			name       	"Precision"
			value      	"2")
		    (object Attribute
			tool       	"Oracle8"
			name       	"Scale"
			value      	"6")
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsIndex"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"IsPrimaryKey"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"CompositeUnique"
			value      	FALSE)
		    (object Attribute
			tool       	"Oracle8"
			name       	"CheckConstraint"
			value      	"")))
	    (object Attribute
		tool       	"Oracle8"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"ComponentTest"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Rose Model Integrator"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"TopLink"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Version Control"
		name       	"HiddenTool"
		value      	FALSE)
	    (object Attribute
		tool       	"Visual Basic"
		name       	"propertyId"
		value      	"783606378")
	    (object Attribute
		tool       	"Visual Basic"
		name       	"default__Class"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Visual Basic"
			name       	"UpdateCode"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"UpdateModel"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"InstancingSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Visual Basic"
				name       	"Private"
				value      	221)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"PublicNotCreatable"
				value      	213)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"SingleUse"
				value      	214)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"GlobalSingleUse"
				value      	215)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"MultiUse"
				value      	219)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"GlobalMultiUse"
				value      	220)))
		    (object Attribute
			tool       	"Visual Basic"
			name       	"BaseSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Visual Basic"
				name       	"(none)"
				value      	222)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"0"
				value      	223)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"1"
				value      	224)))
		    (object Attribute
			tool       	"Visual Basic"
			name       	"OptionBase"
			value      	("BaseSet" 222))
		    (object Attribute
			tool       	"Visual Basic"
			name       	"OptionExplicit"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"OptionCompare"
			value      	("CompareSet" 202))
		    (object Attribute
			tool       	"Visual Basic"
			name       	"Instancing"
			value      	("InstancingSet" 219))
		    (object Attribute
			tool       	"Visual Basic"
			name       	"CompareSet"
			value      	(list Attribute_Set
			    (object Attribute
				tool       	"Visual Basic"
				name       	"(none)"
				value      	202)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"Binary"
				value      	203)
			    (object Attribute
				tool       	"Visual Basic"
				name       	"Text"
				value      	204)))))
	    (object Attribute
		tool       	"Visual Basic"
		name       	"default__Operation"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Visual Basic"
			name       	"LibraryName"
			value      	"")
		    (object Attribute
			tool       	"Visual Basic"
			name       	"AliasName"
			value      	"")
		    (object Attribute
			tool       	"Visual Basic"
			name       	"IsStatic"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ProcedureID"
			value      	"")
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ReplaceExistingBody"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"DefaultBody"
			value      	(value Text ""))))
	    (object Attribute
		tool       	"Visual Basic"
		name       	"default__Attribute"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Visual Basic"
			name       	"New"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"WithEvents"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ProcedureID"
			value      	"")
		    (object Attribute
			tool       	"Visual Basic"
			name       	"PropertyName"
			value      	"")
		    (object Attribute
			tool       	"Visual Basic"
			name       	"Subscript"
			value      	"")))
	    (object Attribute
		tool       	"Visual Basic"
		name       	"default__Role"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Visual Basic"
			name       	"UpdateCode"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"New"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"WithEvents"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"FullName"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ProcedureID"
			value      	"")
		    (object Attribute
			tool       	"Visual Basic"
			name       	"PropertyName"
			value      	"")
		    (object Attribute
			tool       	"Visual Basic"
			name       	"Subscript"
			value      	"")))
	    (object Attribute
		tool       	"Visual Basic"
		name       	"default__Inherit"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ImplementsDelegation"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"FullName"
			value      	FALSE)))
	    (object Attribute
		tool       	"Visual Basic"
		name       	"default__Param"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ByVal"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ByRef"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"Optional"
			value      	FALSE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ParamArray"
			value      	FALSE)))
	    (object Attribute
		tool       	"Visual Basic"
		name       	"default__Module-Spec"
		value      	(list Attribute_Set
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ProjectFile"
			value      	"")
		    (object Attribute
			tool       	"Visual Basic"
			name       	"UpdateCode"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"UpdateModel"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ImportReferences"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"QuickImport"
			value      	TRUE)
		    (object Attribute
			tool       	"Visual Basic"
			name       	"ImportBinary"
			value      	FALSE)))
	    (object Attribute
		tool       	"Visual Basic"
		name       	"HiddenTool"
		value      	FALSE))
	quid       	"39C9260C00D9"))

    Contact GitHub API Training Shop Blog About 

    ? 2017 GitHub, Inc. Terms Privacy Security Status Help 

