#Template V3
---
  HiShoot2i v1.2.0

**Content**
---
- [Manifest](#manifest)
- [Config](#config)
- [Download](#download)

---
**Manifest** 

file: [AndroidManifest.xml](src/main/AndroidManifest.xml)

    <manifest xmlns:android="http://schemas.android.com/apk/res/android"
      package="id.ratabb.templatev3.sample">    
	    <application
            android:label="Sample HiShoot2i Template v3"
            android:icon="@mipmap/ic_launcher"
            android:hasCode="false">
            <meta-data
                android:name="org.illegaller.ratabb.hishoot2i.TEMPLATE"
                android:value="3"/>
        </application>
    </manifest>

**Config**

file assets: [template.cfg](src/main/assets/template.cfg)
    
	{
	  "author"            : "template maker",
	  "name"              : "template name",
	  "desc"              : "description",
	
	  "coordinate"        : [
	    162, 257,
	    597, 188,
	    481, 513,
	    987, 414
	  ],
	
	  "template_size"     : {
	      "width"  : 1200,
	      "height" : 840
	  },
	
	  "preview"           : "preview-file-name-without-ext",
	
	  "frame"             : "frame-file-name-without-ext",
	
	  "shadow"            : null,
	
	  "glares"            : [
	    {
	      "name"     : "glare-1-file-name-without-ext",
	      "size"     : {
	        "width"  : 148,
	        "height" : 36
	      },
	      "position" : {
            "x" : 251,
	        "y" : 187
	      }
	    },
        {
	      "name"     : "glare-N-file-name-without-ext",
	      "size"     : {
	        "width"  : 139,
	        "height" : 59
	      },
	      "position" : {
	        "x" : 732,
	        "y" : 470
	      }
	    }
	  ]
	}

- coordinate: screen shoot

		[
          left_top_x, left_top_y,
		  right_top_x, right_top_y,
		  left_bottom_x, left_bottom_y,
		  right_bottom_x, right_bottom_y
		]

- desc (optional) `null` ok

- preview (optional) `null` ok, file name without extention

- shadow (optional) `null` ok, file name without extention

- glares (optional) `null` ok, unlimited count
  - name: file name without extention
  - size: image size
  - position: image position  

**Download**

[Here](sample-v3.apk)