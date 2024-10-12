# Projects

<ul id="projects-list"></ul>

<script>
    function loadProjects() {
        const projectsList = document.getElementById('projects-list');
        const projectElements = document.querySelectorAll('.sublist [id^="project"]');
      
        projectElements.forEach(element => {
            const listItem = document.createElement('li');
            const link = document.createElement('a');
            link.href = element.getAttribute('href');
            link.innerHTML = element.innerHTML;
            listItem.appendChild(link);
            projectsList.appendChild(listItem);
        });
    }
    
    document.addEventListener('DOMContentLoaded', loadProjects);
</script>
