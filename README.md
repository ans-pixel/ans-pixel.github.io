<style>
    h3 {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: bold;

        padding: 360px 0px;
    }

    h4 {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: bold;

        padding: 36px 0px;
    }

    p {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 500;

        line-height: 30px;
        font-size: 16px
    }

    ul {
        list-style-type: disc;
    }

    #li_auth {
        font-size: 16px;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 500;

        line-height: 30px;
        padding: 12px 0px;
    }

    .guide_accordion {
        background-color: #e9ecef;
        color: black;
        cursor: pointer;
        padding-left: 28px;
        padding-top: 20px;
        padding-bottom: 20px;
        padding-right: 28px;
        width: 100%;
        text-align: left;
        border: none;
        transition: 0.4s;

        font-size: 24px;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 700;

        letter-spacing: 1.5px;
    }

    .guide_accordion:hover {
        background-color: #adb5bd;
    }

    .guide_panel {
        padding: 18px 36px;
        background-color: white;

        text-align: justify;
        font-size: 18px;
        line-height: 30px;

        border-radius: 10px;
        overflow: hidden;
        transition: all 1s ease;
    }
</style>

<button class="guide_accordion">Policies</button>
<div class="guide_panel" style="max-height: 0; padding: 0 36px">
    <p>These are our test policies.</p>
</div>
<br>
<button class="guide_accordion">Work-Life Balance, Working Hours, and Mental Health and Well-Being</button>
<div class="guide_panel" style="max-height: 0; padding: 0 36px">
</div>
<br>
<button class="guide_accordion">Responsibilities, Expectations and Training</button>
<div class="guide_panel" style="max-height: 0; padding: 0 36px">
</div>

<script>
    var acc = document.getElementsByClassName("guide_accordion");
    var i;

    for (i = 0; i < acc.length; i++) {
        acc[i].addEventListener("click", function () {
            this.classList.toggle("active");

            var panel = this.nextElementSibling;
            if (panel.style.maxHeight != "0px") {
                panel.style.maxHeight = "0px";
                panel.style.padding = "0px 36px";
            }
            else {
                panel.style.maxHeight = panel.scrollHeight + "px";
                panel.style.padding = "18px 36px";
            }
        });
    }
</script>
