# PhD.Hub Website Development Progress

## Project Overview
Building a bilingual (Vietnamese/English) website for PhD.Hub - an academic community founded by Dr. Tran Quoc Thien, connecting 110,000+ members to share scholarships, academic experiences, and support Vietnamese students worldwide.

## Completed Features

### 1. Foundation Page (`foundation.html`)
- ✅ Changed background color to beige (#faf9f6) for Programs section
- ✅ Styled program cards with value-card class (matching Values section style)
- ✅ Added clickable modal dialogs for 6 programs:
  1. "Ngọn cuồn sách - Vạn ước mơ" (Clean Books - Dream Oars)
  2. Visa Fee Support
  3. FREE Mentorship
  4. Mentor-Mentee Matching
  5. University Entrance Exam Prep
  6. Encouragement Scholarships
- ✅ Added "Learn More →" / "Tìm hiểu thêm →" text to all cards
- ✅ Implemented full bilingual support for all modals
- ✅ Modal features:
  - Fade-in animation with backdrop blur
  - Close on click outside or Escape key
  - Responsive design (max-width: 900px)
  - Prevents background scrolling when open
- ✅ Modal content includes:
  - Program images (program_2.webp, program_3.webp)
  - External links (Thanh Niên news, YouTube videos, Google Forms)
  - Styled buttons for calls-to-action
- ✅ Updated Programs section description (removed sponsorship note from description)
- ✅ Modal content for each program:
  - Modal 1: Full description + Thanh Niên article link + YouTube video link
  - Modal 2: Eligibility, Support, Budget details + program image + application form
  - Modal 3: Description + program image + application form
  - Modals 4-6: Launch dates only

### 2. About Page (`about.html`)
- ✅ Replaced "Our Story" section with Dr. Thien's personal message
- ✅ Single-column layout with text followed by image (1.webp)
- ✅ Updated "Our Values" to "Scientific Background" section
- ✅ Added Dr. Thien's academic credentials and achievements
- ✅ Added Google Scholar link placeholder
- ✅ Added image 2.webp to Scientific Background section
- ✅ Increased paragraph spacing (24px) for better readability
- ✅ Full bilingual support for all content

### 3. Mentorship Page (`mentorship.html`)
- ✅ Added MacroMentorship section at the top
- ✅ Added FREE Mentorship registration button
- ✅ Added 2 YouTube success story links (buttons):
  - Nguyễn Đức Thăng - Purdue University
  - Lâm Ngọc Ngân - University of Warwick
- ✅ Replaced "How It Works" with "Một số học trò tiêu biểu" (Outstanding Students)
- ✅ Created 15 student profile cards in 2-column responsive grid:
  1. Lâm Ngọc Ngân - UT Austin (PhD Biomedical Science)
  2. Nguyễn Ngọc Phúc Tiên - UPenn (MSc Electrical Engineering)
  3. Nguyễn Văn Thắng - Virginia Tech (PhD Materials Science)
  4. Đoàn Trung Vương - UTS Sydney (PhD Materials Science)
  5. Lê Minh Triết - NTU Singapore (PhD Civil Engineering)
  6. Lai Quốc Huy - UMass Amherst (PhD Civil & Environmental Engineering)
  7. Nguyễn Minh Hương - NJIT (PhD UI/UX Design)
  8. Đặng Võ Hiệp - UVA (PhD Environmental Science)
  9. Liễu Phước Long - WSU Pullman (PhD Food Science)
  10. Nguyễn Đức Thăng - Purdue (PhD Materials Science)
  11. Xiang Zhao - MTU (MSc Civil & Environmental Engineering)
  12. Trinh Trần - UCF (PhD Electrical Engineering)
  13. Nhật Trần - UF (PhD Civil & Environmental Engineering)
  14. Nam Nguyễn - Georgia Tech (PhD Civil & Environmental Engineering)
  15. Nguyễn Ngọc Linh - MTU (PhD Civil & Environmental Engineering)
- ✅ Each student card includes:
  - Individual photo (1.webp - 15.webp)
  - Name and graduation year
  - Scholarship type
  - University link to US News or official website
  - Major/field of study
  - Additional scholarships (where applicable)
- ✅ Full bilingual support for all student profiles
- ✅ Mobile-responsive grid (minmax(280px, 1fr))

### 4. Navigation & Site-wide Changes
- ✅ Removed "Scholarship News" from navigation menu on all pages:
  - index.html
  - about.html
  - foundation.html
  - mentorship.html
- ✅ Removed "Scholarship News" from footer on all pages
- ✅ Set Vietnamese as default language on all pages
- ✅ Dark mode support maintained throughout

### 5. CSS Styling
- ✅ Added modal styles:
  - `.modal` - Hidden by default, full-screen overlay
  - `.modal-content` - Centered card with max-width 900px
  - `.modal-close` - X button in top right
  - `.modal-link` - Styled external links with hover effects
- ✅ Added `.card-learn-more` styles for program cards
- ✅ Mobile-responsive styling for all sections
- ✅ Beige background for sections: `#faf9f6`

### 6. JavaScript Functionality
- ✅ Modal functions:
  - `openModal(modalId)` - Shows modal and prevents body scroll
  - `closeModal(modalId)` - Hides modal and restores scroll
  - Click outside modal to close
  - Press Escape key to close
- ✅ Language toggle functionality working with all new content
- ✅ Vietnamese set as default language

### 7. Assets Organization
- ✅ Images added:
  - `assets/images/foundation/program_2.webp` (Visa Support)
  - `assets/images/foundation/program_3.webp` (Mentorship)
  - `assets/images/about/1.webp` (Our Story)
  - `assets/images/about/2.webp` (Scientific Background)
  - `assets/images/mentorship/1.webp` - `15.webp` (Student photos)

### 8. GitHub Pages Setup
- ✅ Repository: `mnguyen0226/mnguyen0226swetest-phdhub`
- ✅ Instructions provided for GitHub Pages deployment
- ✅ Confirmed free hosting eligibility (public repository)
- ✅ Site will be available at: `https://mnguyen0226.github.io/mnguyen0226swetest-phdhub/`

### 9. Deleted/Removed
- ✅ Removed unnecessary `mnguyen0226swetest-phdhub` subfolder (duplicate/template)
- ✅ `scholarship.html` file exists but is not linked anywhere

## Technical Stack
- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Icons**: Font Awesome 6.4.0
- **Hosting**: GitHub Pages (free)
- **Features**: 
  - Bilingual support (Vietnamese/English)
  - Dark mode toggle
  - Responsive design
  - Modal dialogs
  - Smooth animations

## Key Design Patterns
1. **Bilingual Content**: Using `data-en` and `data-vi` attributes
2. **Modals**: Hidden by default, shown with display: flex
3. **Responsive Grid**: `grid-template-columns: repeat(auto-fit, minmax(280px, 1fr))`
4. **Color Scheme**:
   - Primary: Blue (#2563eb)
   - Beige Background: #faf9f6
   - Text adapts to light/dark mode
5. **Default Language**: Vietnamese (set via localStorage)

## External Links Integration
- ✅ Thanh Niên news article
- ✅ YouTube videos (2 student success stories + 1 program video)
- ✅ Google Forms (3 application forms)
- ✅ US News university rankings
- ✅ University official websites
- ✅ Facebook group & personal page
- ✅ Email contact

## Browser Compatibility
- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile-responsive (tested for phone, tablet, desktop)
- Dark mode support

## Future Considerations
- Custom domain setup (optional)
- Google Scholar profile link update needed
- `scholarship.html` can be deleted if not needed
- Additional student profiles can be added following existing pattern

## Notes
- All content is fully bilingual (Vietnamese primary, English secondary)
- Site operates entirely on client-side (no backend required)
- Free to host and maintain on GitHub Pages
- Images use `.webp` format for optimization