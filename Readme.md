# Features
This simple Web App let's you mark some notes to remember using *local storage* of your browser.
''' javascript
 <script>
        function getNote(){
            if(localStorage.getItem('note')){
                var note=localStorage.getItem('note');
            }else{
                var note='What do you want to remember?';  
            }
            document.getElementById('note').innerHTML=note;
            
        }
        function saveNote(id){
            var note=document.getElementById('note').innerHTML;
            localStorage.setItem('note',note);
        }
        
        function clearNote(){
            clear: localStorage.clear();
            return false;
        }
    </script>
    '''
