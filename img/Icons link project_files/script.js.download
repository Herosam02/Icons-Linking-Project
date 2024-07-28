// turn pages when click next or prev button
const pagesTurnBtn = document.querySelectorAll('.nextprev-btn');

pagesTurnBtn.forEach((el, index) => {
  el.onclick = () => {
    const pagesTurnid = el.getAttribute('data-page')
    const pagesTurn = document.getElementById(pagesTurnid)

    if (pagesTurn.classList.contains('turn')) {
      pagesTurn.classList.remove('turn')
      setTimeout(() => {
        pagesTurn.style.zIndex = 20 - index;
      }, 500)
    }
    else {
      pagesTurn.classList.add('turn')
      setTimeout(() => {
        pagesTurn.style.zIndex = 20 + index;
      }, 500)
    }
  }
})

// contact me button when click
const pages = document.querySelectorAll('.book-page.page-right');
const contactMeBtn = document.querySelector('.btn.contact-me');

contactMeBtn.onclick = (pages) => {
  pages.forEach((page, index) => {
    setTimeout(() => {
      page.classList.add('turn');

      setTimeout(() => {
        page.style.zIndex = 20 - index;
      }, 500)
    }, (index + 1) * 400 + 100)
  })
}

//creat reverse index function
let totalPages = pages.length;
let pageNumber = 0;

function reverseIndex() {
  pageNumber--;
  if (pageNumber < 0){
    pageNumber = totalPages - 1;
  }
}