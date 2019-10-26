# mysql-workbench-monokai-theme

DYI to apply monokai theme on MySQL Workbench

# Instructions

This instructions are based on Mysql Workbench installs from .deb packages for Ubuntu 18.04

1. Locate the file `code_editor.xml` under `/usr/share/mysql-workbench/data` 

    ```bash
    cd /usr/share/mysql-workbench/data
    ```
2. Create a backup copy of it

    ```bash
    sudo copy code_editor.xml code_editor.xml.backup
    ```
3. Edit the `code_editor.xml` file with your favorite text editor    ```

    ```bash
    sudo vim code_editor.xml
    ```
4. replace the `style` nodes with the following
    ```xml
    <!-- 
        dark-gray:         #282828;
        brown-gray:        #49483E;
        gray:              #888888;
        light-gray:        #CCCCCC;
        ghost-white:       #F8F8F0;
        light-ghost-white: #F8F8F2;
        yellow:            #E6DB74;
        blue:              #66D9EF;
        pink:              #F92672;
        purple:            #AE81FF;
        brown:             #75715E;
        orange:            #FD971F;
        light-orange:      #FFD569;
        green:             #A6E22E;
        sea-green:         #529B2F; 
    -->

    <style id="32" fore-color="#DDDDDD" back-color="#282828" bold="No" />   <!-- STYLE_DEFAULT       !BACKGROUND!   -->
    <style id="33" fore-color="#DDDDDD" back-color="#282828" bold="No" />   <!-- STYLE_LINENUMBER                   -->
    <style id= "0" fore-color="#DDDDDD" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_DEFAULT                  -->

    <style id= "1" fore-color="#999999" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_COMMENT                  -->
    <style id= "2" fore-color="#999999" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_COMMENTLINE              -->
    <style id= "3" fore-color="#DDDDDD" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_VARIABLE                 -->
    <style id= "4" fore-color="#66D9EF" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_SYSTEMVARIABLE           -->
    <style id= "5" fore-color="#66D9EF" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_KNOWNSYSTEMVARIABLE      -->
    <style id= "6" fore-color="#AE81FF" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_NUMBER                   -->
    <style id= "7" fore-color="#F92672" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_MAJORKEYWORD             -->
    <style id= "8" fore-color="#F92672" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_KEYWORD                  -->
    <style id= "9" fore-color="#9B859D" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_DATABASEOBJECT           -->
    <style id="10" fore-color="#DDDDDD" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_PROCEDUREKEYWORD         -->
    <style id="11" fore-color="#E6DB74" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_STRING                   -->
    <style id="12" fore-color="#E6DB74" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_SQSTRING                 -->
    <style id="13" fore-color="#E6DB74" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_DQSTRING                 -->
    <style id="14" fore-color="#F92672" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_OPERATOR                 -->
    <style id="15" fore-color="#9B859D" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_FUNCTION                 -->
    <style id="16" fore-color="#DDDDDD" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_IDENTIFIER               -->
    <style id="17" fore-color="#E6DB74" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_QUOTEDIDENTIFIER         -->
    <style id="18" fore-color="#529B2F" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_USER1                    -->
    <style id="19" fore-color="#529B2F" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_USER2                    -->
    <style id="20" fore-color="#529B2F" back-color="#282828" bold="No" />   <!-- SCE_MYSQL_USER3                    -->
    <style id="21" fore-color="#66D9EF" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_HIDDENCOMMAND            -->
    <style id="22" fore-color="#909090" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_PLACEHOLDER              -->
    <!-- All styles again in their variant in a hidden command -->
    <style id="65" fore-color="#999999" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_COMMENT                  -->
    <style id="66" fore-color="#999999" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_COMMENTLINE              -->
    <style id="67" fore-color="#DDDDDD" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_VARIABLE                 -->
    <style id="68" fore-color="#66D9EF" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_SYSTEMVARIABLE           -->
    <style id="69" fore-color="#66D9EF" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_KNOWNSYSTEMVARIABLE      -->
    <style id="70" fore-color="#AE81FF" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_NUMBER                   -->
    <style id="71" fore-color="#F92672" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_MAJORKEYWORD             -->
    <style id="72" fore-color="#F92672" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_KEYWORD                  -->
    <style id="73" fore-color="#9B859D" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_DATABASEOBJECT           -->
    <style id="74" fore-color="#DDDDDD" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_PROCEDUREKEYWORD         -->
    <style id="75" fore-color="#E6DB74" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_STRING                   -->
    <style id="76" fore-color="#E6DB74" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_SQSTRING                 -->
    <style id="77" fore-color="#E6DB74" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_DQSTRING                 -->
    <style id="78" fore-color="#F92672" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_OPERATOR                 -->
    <style id="79" fore-color="#9B859D" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_FUNCTION                 -->
    <style id="80" fore-color="#DDDDDD" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_IDENTIFIER               -->
    <style id="81" fore-color="#E6DB74" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_QUOTEDIDENTIFIER         -->
    <style id="82" fore-color="#529B2F" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_USER1                    -->
    <style id="83" fore-color="#529B2F" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_USER2                    -->
    <style id="84" fore-color="#529B2F" back-color="#49483E" bold="No" />   <!-- SCE_MYSQL_USER3                    -->
    <style id="85" fore-color="#66D9EF" back-color="#888888" bold="No" />   <!-- SCE_MYSQL_HIDDENCOMMAND            -->
    <style id="86" fore-color="#AAAAAA" back-color="#888888" bold="No" />   <!-- SCE_MYSQL_PLACEHOLDER              -->
    ```
    
    # Authors
    
    I'm not the author for this, just compiled it from a Stack Overflow post, kudos to [Gaston Martinez](https://stackoverflow.com/users/5236061/gaston-martinez) and  [Carlos Mestre](https://stackoverflow.com/users/1555581/elmestre) for their answer on this [Stack Overflow question](https://stackoverflow.com/questions/38088086/change-syntax-highlight-colors-in-mysqlworkbench)
