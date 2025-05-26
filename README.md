## greenShare


<details>
<summary>
  라즈베리파이, 파이썬 기반 스마트팜 IoT 기기 개발 및 센서 자동제어 알고리즘
</summary>
   토글 안 내용
</details>

<details>
<summary>
  React 기반 스마트팜 IoT 기기 연동 및 식물 커뮤니티 웹 구축
</summary>
   토글 안 내용
</details>

<details>
<summary>
  React 기반 스마트팜 IoT 기기 연동 및 식물 커뮤니티 앱 구축
</summary>

<h3>프로젝트 개요</h3>
<p>관리자는 작물 재배 환경과 적정환경 비교 & 농장 자동화 제공
일반 사용자는 노하우를 공유하고 소통을 통해 작물을 키울때 드는 불편함 해소</p>


![Image](https://github.com/user-attachments/assets/2f2eb122-e754-4101-9594-07f90f3ad691)


</details>

function convertBlockquotesToCallouts() {
    const blockquotes = document.querySelectorAll('blockquote[data-ke-style="style1"]');
    const CALLOUT_CLASSES = {
        '[!CAUTION]': 'markdown-callout-caution',
        '[!WARNING]': 'markdown-callout-warning',
        '[!NOTE]': 'markdown-callout-note',
        '[!TIP]': 'markdown-callout-tip',
        '[!IMPORTANT]': 'markdown-callout-important'
    };
    const CALLOUT_TITLES = {
        '[!CAUTION]': '⛔ 경고',
        '[!WARNING]': '⚠️ 주의',
        '[!NOTE]': '📝 참고',
        '[!TIP]': '💡 팁',
        '[!IMPORTANT]': '❗ 중요'
    };
    blockquotes.forEach(blockquote => {
        const calloutParagraph = blockquote.children[1]; // 티스토리 자동 생성 문단 무시
        if (!calloutParagraph) return;

        const calloutTitle = calloutParagraph.textContent.trim();
        const calloutClass = CALLOUT_CLASSES[calloutTitle];
        if (!calloutClass) return;

        blockquote.classList.add('markdown-callout', calloutClass);
        calloutParagraph.classList.add('callout-title');
        calloutParagraph.innerHTML = `${CALLOUT_TITLES[calloutTitle]}`;
    })
} 
