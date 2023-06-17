# HTML
### <a> Anchor Tag
  **function**    :     creates hypertext for any URL
  
  **Syntax**      :     `<a href = [url]> the_display_word </a>`
  
  #### Example     :     
     <a href = Google.com> Google </a>
  
 **Output**
>  <a href = Google.com> Google </a>  
  
  ### Attributes
  
1.   **_href_**
      -   includes URL
            - Sections of a page
            - Telephone numbers `tel: URLs'`
            - Email Addresses   `mailto: URLs'`           
1.   **_rel_**
      -   the relation of linked URLs'
  

### <abbr> Abbreviation Tag
  **function**    :     marking up an abbreviation and acronym semantically
  
  **Syntax**      :     `<p> sample_text <abbr> abbreviation/acronym <abbr/> more_text</p>`
  
  #### Example   :     
>       <p>We are learning <abbr>HTML</abbr> for fun.</p>
  
  #### Output
>  <p>We are learning <abbr>HTML</abbr> for fun.</p>
  
  **Note**: Computer now understands **HTML** as _abbreviation._
  
  ### Attributes
  1.   **_title_** 
        -  expansion of the abbreviation
        -   in case a user searches the expanded form of the abbreviation _title tag_ helps computer to fetch even those results where only abbreviation or arcronym is present.
        - it is usually used with `<dfn>` tag to semantise the _definition, expansion of abbreviation and abbreviation_ itself.
        - it would help search engines to find the most apprepriate answers first
  
#### Example   :     
>       <p><dfn><abbr title= "Hyper Text Markup Language">HTML</abbr> is a markup language</dfn></p>
  
#### Output
>  <p><dfn><abbr title= "Hyper Text Markup Language">HTML</abbr> is a markup language</dfn></p>
  
>   **Note**: Computer now understands **HTML** as _abbreviation._ And stores it's _expandable form_ as **Hyper Text Markup Language.**
  
### Address tag

**function**        :       provides content information
                                - physical address, URL, email, number, social media, etc.
  
**syntax**          :       `<address>text</address>`
  
  #### Example   :  
  
  ```
    <address>
      Contact the author at <a href ="https://www.linkedin.com/"> Linkedin </a> <br>
      Visit us: <br>
      1st Street <br>
      xyz Town <br>
      Delhi-110001 <br>
      India
   </address>
  ```
  

#### Output
<address>
      Contact the author at <a href ="https://www.linkedin.com/"> Linkedin </a> <br>
      Visit us: <br>
      1st Street <br>
      xyz Town <br>
      Delhi-110001 <br>
      India
   </address>
  
### Article tag
  
**function**      :     it specifies independent self contained content
  
**Syntax**        :     `<article class="sample-classname"> components and text </article>`
  
#### Example     :     

```
  <article class="forecast">
    <h1>Weather Forecast</h1>
    <artcile class="day-forecast">
      <h2> 3 MARCH</h2>
      <p>Rain</p>
      </article>
    <article class="day-forecast">
      <h2>4 MARCH</h2>
      <p>Sun</p>
    </article>
    <article class="day-forecast">
      <h2> 5 March </h2>
      <p> Heavy Rain </p>
 </article>
    
```

#### Output
 <div style="background-color:blue">  
  <article class="forecast" style="background-colour: red;">
    <h1>Weather Forecast</h1>
    <artcile class="day-forecast">
      <h2> 3 MARCH</h2>
      <p>Rain</p>
      </article>
    <article class="day-forecast">
      <h2>4 MARCH</h2>
      <p>Sun</p>
    </article>
    <article class="day-forecast">
      <h2> 5 March </h2>
      <p> Heavy Rain </p>
   </article>
 </div>

### Audio tag
**function**      :       The `<audio>`` HTML element is used to embed sound content in documents. It may contain one or more audio sources
   
**syntax**        :       `<audio src="source"></audio>`

### Attributes
     
1. src
    - The URL of the audio to embed.
     
1. **_controls_**
    - If this attribute is present, the browser will offer controls to allow the user to control audio playback, including volume, seeking, and pause/resume playback.

1. **_muted_**
   - A Boolean attribute that indicates whether the audio will be initially silenced. Its default value is false.
     
1. **_preload_**
    - This enumerated attribute is intended to provide a hint to the browser about what the author thinks will lead to the best user experience. It may have one of the following values:

    >  **Note** Use _metadata_ as the value for preload. 
     
        - none: Indicates that the audio should not be preloaded.
        - metadata: Indicates that only audio metadata (e.g. length) is fetched.
        - auto: Indicates that the whole audio file can be downloaded, even if the user is not expected to use it.
        - empty string: A synonym of the auto value.

1. **_loop_** (replay)
     -A Boolean attribute: if specified, the audio player will automatically seek back to the start upon reaching the end of the audio.
     
  
