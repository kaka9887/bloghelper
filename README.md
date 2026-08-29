# bloghelper
블로그 관리를 하기 위해 만듬

<!doctype html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="color-scheme" content="light dark">
  <title>개인정보처리방침 | 네이버 블로그 통합 도우미</title>
  <style>
    :root {
      color-scheme: light dark;
      --bg: #f6f8fa;
      --card: #ffffff;
      --text: #24292f;
      --muted: #57606a;
      --line: #d0d7de;
      --accent: #0969da;
      --soft: #ddf4ff;
      --soft-text: #0550ae;
      --warn-bg: #fff8c5;
      --warn-text: #633c01;
    }
    @media (prefers-color-scheme: dark) {
      :root {
        --bg: #0d1117;
        --card: #161b22;
        --text: #e6edf3;
        --muted: #9da7b3;
        --line: #30363d;
        --accent: #58a6ff;
        --soft: #0c2d48;
        --soft-text: #a5d6ff;
        --warn-bg: #3b2e00;
        --warn-text: #f2cc60;
      }
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      background: var(--bg);
      color: var(--text);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans KR", Arial, sans-serif;
      line-height: 1.7;
      word-break: keep-all;
    }
    main {
      width: min(920px, calc(100% - 32px));
      margin: 48px auto;
      padding: 44px 48px;
      background: var(--card);
      border: 1px solid var(--line);
      border-radius: 16px;
      box-shadow: 0 8px 28px rgba(0,0,0,.06);
    }
    h1 { margin: 0 0 8px; font-size: 32px; letter-spacing: -.5px; }
    h2 { margin: 42px 0 12px; padding-top: 6px; font-size: 21px; }
    h3 { margin: 24px 0 8px; font-size: 17px; }
    p { margin: 10px 0; }
    ul { margin: 8px 0 8px 22px; padding: 0; }
    li { margin: 6px 0; }
    a { color: var(--accent); }
    .meta { color: var(--muted); font-size: 14px; }
    .summary {
      margin: 28px 0;
      padding: 18px 20px;
      border-radius: 12px;
      background: var(--soft);
      color: var(--soft-text);
    }
    .summary strong { display: block; margin-bottom: 5px; }
    .notice {
      padding: 14px 16px;
      border: 1px solid var(--line);
      border-radius: 10px;
      color: var(--muted);
      font-size: 14px;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 14px 0 20px;
      font-size: 14px;
    }
    th, td {
      border: 1px solid var(--line);
      padding: 12px 14px;
      vertical-align: top;
      text-align: left;
    }
    th { background: color-mix(in srgb, var(--card) 84%, var(--muted) 16%); }
    code {
      padding: 2px 5px;
      border: 1px solid var(--line);
      border-radius: 5px;
      font-family: ui-monospace, SFMono-Regular, Menlo, Consolas, monospace;
      font-size: 90%;
    }
    footer {
      margin-top: 48px;
      padding-top: 22px;
      border-top: 1px solid var(--line);
      color: var(--muted);
      font-size: 13px;
    }
    @media (max-width: 680px) {
      main { margin: 0; width: 100%; padding: 30px 20px; border: 0; border-radius: 0; }
      h1 { font-size: 27px; }
      table, thead, tbody, tr, th, td { display: block; }
      thead { display: none; }
      tr { border: 1px solid var(--line); margin-bottom: 12px; border-radius: 8px; overflow: hidden; }
      td { border: 0; border-bottom: 1px solid var(--line); }
      td:last-child { border-bottom: 0; }
      td::before { content: attr(data-label); display: block; font-weight: 700; margin-bottom: 4px; }
    }
  </style>
</head>
<body>
<main>
  <header>
    <h1>개인정보처리방침</h1>
    <p><strong>네이버 블로그 통합 도우미</strong></p>
    <p class="meta">시행일: 2026년 8월 29일 · 대상 버전: Chrome Extension V2.4.25 이상</p>
  </header>

  <section class="summary">
    <strong>핵심 요약</strong>
    네이버 블로그 통합 도우미는 확장 프로그램의 기능 제공에 필요한 범위에서만 데이터를 처리합니다.
    블로그 관리 데이터와 설정은 주로 사용자의 Chrome 확장 프로그램 저장소에 보관되며, 로그인·라이선스 확인에는 Supabase를 사용합니다.
    사용자가 AI 댓글/답글 기능을 활성화한 경우에만 해당 기능 수행에 필요한 블로그 본문 또는 댓글 정보가 사용자가 등록한 Gemini API 키를 이용해 Google Gemini API로 전송됩니다.
    사용자 데이터를 광고, 데이터 판매 또는 신용평가 목적으로 사용하지 않습니다.
  </section>

  <h2>1. 처리하는 정보와 이용 목적</h2>
  <table>
    <thead>
      <tr><th>구분</th><th>처리되는 정보</th><th>이용 목적</th><th>주요 저장/전송 위치</th></tr>
    </thead>
    <tbody>
      <tr>
        <td data-label="구분">확장 프로그램 계정 및 인증</td>
        <td data-label="처리되는 정보">이메일 주소, 로그인 시 입력한 비밀번호, 사용자 ID, 인증 토큰</td>
        <td data-label="이용 목적">확장 프로그램 로그인, 세션 유지, 사용자 및 라이선스 상태 확인, 비밀번호 변경</td>
        <td data-label="주요 저장/전송 위치">Supabase 인증 서버 및 사용자의 브라우저 저장소. 비밀번호는 인증/변경 요청을 위해 전송되며 확장 프로그램이 평문 비밀번호를 지속 저장하지 않습니다.</td>
      </tr>
      <tr>
        <td data-label="구분">기기 및 라이선스 정보</td>
        <td data-label="처리되는 정보">임의 생성 설치 ID, 확장 프로그램 ID/버전, 브라우저 플랫폼을 기반으로 한 기기 표시명, 기기 공개키, 라이선스 상태 및 허용 기기 수 관련 정보</td>
        <td data-label="이용 목적">무단 사용 방지, 사용자별 기기 등록 및 라이선스 검증, 버전 요구사항 확인</td>
        <td data-label="주요 저장/전송 위치">Supabase 기반 인증/라이선스 서버 및 브라우저 저장소</td>
      </tr>
      <tr>
        <td data-label="구분">확장 프로그램 설정</td>
        <td data-label="처리되는 정보">자동화 옵션, 실행 간격, 기능 ON/OFF 상태, UI 설정, AI 댓글 슬롯 사용량, 사용자가 입력한 Gemini API 키 등</td>
        <td data-label="이용 목적">사용자 설정 유지 및 확장 프로그램 기능 제공</td>
        <td data-label="주요 저장/전송 위치">Chrome <code>storage.local</code>, <code>storage.sync</code>, <code>storage.session</code> 등. Gemini API 키는 브라우저 로컬 저장소에 저장되고 Gemini API 요청 인증에 사용됩니다.</td>
      </tr>
      <tr>
        <td data-label="구분">네이버 블로그 페이지/관리 정보</td>
        <td data-label="처리되는 정보">블로그 ID, 닉네임, 게시글 URL/번호/제목/본문 텍스트, 댓글 및 답글 관련 정보, 이웃/댓글 작성자 정보, 관리 목록 및 자동화 진행 상태</td>
        <td data-label="이용 목적">공감·댓글·답글 보조, 이웃 관리, 댓글 작성자 관리, 자동화 대상 판별 및 사용자가 요청한 블로그 관리 기능 수행</td>
        <td data-label="주요 저장/전송 위치">정보의 상당 부분은 사용자의 브라우저에서 처리되거나 Chrome 로컬 저장소에 저장됩니다. 사용자가 요청한 네이버 기능 수행 시 네이버 서비스와 통신합니다.</td>
      </tr>
      <tr>
        <td data-label="구분">AI 댓글/답글 생성 정보</td>
        <td data-label="처리되는 정보">AI 분석에 필요한 게시글 본문 일부, 게시글 제목, 감지된 장소명, 이미지 개수, 댓글 작성자 닉네임, 원댓글 내용 등 기능별 필요한 정보</td>
        <td data-label="이용 목적">게시글 내용에 맞는 AI 댓글 후보 또는 원댓글에 대한 AI 답글 생성</td>
        <td data-label="주요 저장/전송 위치">사용자가 AI 기능을 활성화한 경우 Google Gemini API로 전송됩니다. 현재 확장 프로그램은 댓글 생성을 위해 게시글 이미지 파일 자체를 Gemini API로 전송하지 않고 텍스트 및 필요한 메타정보를 사용합니다.</td>
      </tr>
    </tbody>
  </table>

  <h2>2. 네이버 블로그 접근 범위</h2>
  <p>확장 프로그램은 공개된 핵심 기능을 수행하기 위해 다음 네이버 블로그 관련 페이지에 접근할 수 있습니다.</p>
  <ul>
    <li><code>blog.naver.com</code>, <code>m.blog.naver.com</code>: 게시글 확인, 공감·댓글·답글 보조 및 자동화 기능</li>
    <li><code>section.blog.naver.com</code>: 이웃 새글 및 자동화 대상 게시글 확인</li>
    <li><code>admin.blog.naver.com</code>: 이웃 및 댓글 작성자 등 블로그 관리 기능</li>
  </ul>
  <p>확장 프로그램은 사용자가 Chrome에서 이미 로그인한 네이버 세션을 이용해 사용자가 요청한 기능을 수행하며, 네이버 계정 비밀번호를 별도로 수집하거나 저장하기 위한 기능을 제공하지 않습니다.</p>

  <h2>3. 외부 서비스로의 전송 및 처리</h2>
  <p>확장 프로그램의 단일 목적 및 사용자가 요청한 기능을 제공하기 위해 다음 외부 서비스와 데이터가 통신할 수 있습니다.</p>
  <table>
    <thead>
      <tr><th>서비스</th><th>목적</th><th>전송될 수 있는 정보</th></tr>
    </thead>
    <tbody>
      <tr>
        <td data-label="서비스">Supabase</td>
        <td data-label="목적">확장 프로그램 계정 인증, 세션 갱신, 라이선스 및 기기 인증</td>
        <td data-label="전송될 수 있는 정보">이메일/로그인 인증 정보, 사용자 ID, 인증 토큰, 설치 ID, 확장 프로그램 ID/버전, 기기 표시명, 공개키, 라이선스 검증용 서명 정보 등</td>
      </tr>
      <tr>
        <td data-label="서비스">Google Gemini API</td>
        <td data-label="목적">사용자가 켠 AI 댓글 및 AI 답글 생성</td>
        <td data-label="전송될 수 있는 정보">Gemini API 키, 게시글 본문 일부 및 제목/장소명/이미지 개수 등의 메타정보, 답글 생성 시 닉네임 및 원댓글 내용</td>
      </tr>
      <tr>
        <td data-label="서비스">NAVER</td>
        <td data-label="목적">사용자가 요청한 네이버 블로그 열람·관리·공감·댓글 등 기능 수행</td>
        <td data-label="전송될 수 있는 정보">해당 기능 수행에 필요한 네이버 블로그 요청 정보 및 사용자의 기존 네이버 로그인 세션에 기반한 요청</td>
      </tr>
    </tbody>
  </table>
  <p>각 외부 서비스에서의 데이터 처리는 해당 서비스의 약관 및 개인정보 관련 정책의 적용을 받을 수 있습니다.</p>
  <ul>
    <li><a href="https://supabase.com/privacy" target="_blank" rel="noopener noreferrer">Supabase Privacy Policy</a></li>
    <li><a href="https://policies.google.com/privacy" target="_blank" rel="noopener noreferrer">Google Privacy Policy</a></li>
    <li><a href="https://ai.google.dev/gemini-api/terms" target="_blank" rel="noopener noreferrer">Google Gemini API Terms</a></li>
    <li><a href="https://policy.naver.com/policy/privacy.html" target="_blank" rel="noopener noreferrer">NAVER 개인정보처리방침</a></li>
  </ul>

  <h2>4. 로컬 저장 정보</h2>
  <p>확장 프로그램의 편의 기능을 위해 일부 정보는 사용자의 Chrome 프로필에 저장됩니다. 여기에는 확장 프로그램 설정, 자동화 상태, 블로그 ID/이웃/댓글 작성자 관리 데이터, AI 댓글 슬롯 사용량, Gemini API 키 등이 포함될 수 있습니다.</p>
  <p>로그인 세션의 액세스 토큰은 세션 저장소를 이용하고, 인증 유지에 필요한 정보와 기기 서명 키는 브라우저 저장소 및 IndexedDB를 이용합니다. 기기 서명용 개인키는 브라우저 내에서 서명에 사용되며 서버에는 공개키만 전송됩니다.</p>

  <h2>5. 보유 및 삭제</h2>
  <ul>
    <li><strong>브라우저 로컬 데이터:</strong> 사용자가 설정을 초기화하거나 확장 프로그램 데이터를 삭제할 때까지 보관될 수 있으며, 확장 프로그램 제거 시 Chrome의 확장 프로그램 저장 데이터 정책에 따라 삭제될 수 있습니다.</li>
    <li><strong>세션 정보:</strong> 로그아웃, 세션 만료 또는 브라우저/확장 프로그램의 세션 정리 과정에서 제거됩니다.</li>
    <li><strong>Supabase 계정 및 라이선스 정보:</strong> 계정 및 라이선스 제공에 필요한 기간 동안 보관될 수 있으며, 관련 법령상 보존 의무가 있는 경우 해당 기간 동안 보관할 수 있습니다.</li>
    <li><strong>Google Gemini API로 전송된 정보:</strong> Google의 적용 가능한 Gemini API 약관, 개인정보 관련 정책 및 사용자의 Google API 계정 설정에 따라 처리됩니다.</li>
  </ul>
  <p>계정 또는 서버에 보관된 본인 정보의 삭제를 원하는 경우 아래 문의 방법을 통해 삭제를 요청할 수 있습니다.</p>

  <h2>6. 정보의 판매 및 광고 이용</h2>
  <p>운영자는 확장 프로그램이 처리하는 사용자 데이터를 판매하지 않으며, 맞춤형 광고·리타게팅 광고·관심 기반 광고, 데이터 브로커 제공, 신용평가 또는 대출 심사 목적으로 사용하거나 전송하지 않습니다.</p>

  <h2>7. 사용자 데이터에 대한 사람의 접근</h2>
  <p>운영자는 원칙적으로 사용자의 블로그 콘텐츠 등 사용자 데이터를 사람이 직접 열람하는 방식으로 사용하지 않습니다. 다만 사용자가 특정 데이터에 대한 기술 지원을 명시적으로 요청한 경우, 서비스의 보안 및 악용 방지를 위해 필요한 경우, 또는 법령상 의무를 이행하기 위해 필요한 경우에는 필요한 최소 범위에서 처리할 수 있습니다.</p>

  <h2>8. 보안 조치</h2>
  <ul>
    <li>외부 서버 및 API와의 통신은 HTTPS를 사용합니다.</li>
    <li>로그인 비밀번호를 확장 프로그램 설정값으로 평문 지속 저장하지 않습니다.</li>
    <li>액세스 토큰과 인증 유지 정보를 용도에 따라 세션 저장소와 IndexedDB 등에 분리해 사용합니다.</li>
    <li>기기 인증에 사용되는 개인 서명키는 브라우저 내 비추출(non-extractable) CryptoKey 형태로 사용하며, 서버에는 공개키와 검증에 필요한 정보만 전달합니다.</li>
    <li>사용자는 Gemini API 키가 포함된 Chrome 사용자 프로필 및 기기에 대한 접근을 적절하게 보호해야 합니다.</li>
  </ul>

  <h2>9. Chrome Web Store Limited Use 준수</h2>
  <p>네이버 블로그 통합 도우미는 Chrome Web Store User Data Policy 및 Limited Use 요구사항에 따라, 사용자 데이터의 수집·사용·전송을 확장 프로그램에 공개된 단일 목적과 사용자에게 제공되는 기능을 수행하거나 해당 기능의 보안·신뢰성을 유지하는 데 필요한 범위로 제한합니다.</p>
  <p>사용자 데이터는 개인정보처리방침에서 공개한 목적 외에는 사용하지 않으며, 허용되지 않은 광고·판매·재판매 또는 데이터 브로커 제공 목적으로 사용하지 않습니다.</p>

  <h2>10. 개인정보처리방침 변경</h2>
  <p>확장 프로그램 기능 또는 데이터 처리 방식이 변경되는 경우 이 개인정보처리방침을 갱신할 수 있습니다. 사용자 데이터의 처리 목적이나 외부 전송 방식에 중대한 변경이 있는 경우 Chrome Web Store 등록 정보 또는 확장 프로그램 UI 등 적절한 방법으로 변경 사항을 알립니다.</p>

  <h2>11. 문의 및 삭제 요청</h2>
  <div class="notice">
    <p><strong>서비스명:</strong> 네이버 블로그 통합 도우미</p>
    <p><strong>운영자:</strong> 카카</p>
    <p><strong>개인정보 문의/삭제 요청 이메일:</strong> <a href="mailto:kaka9887@naver.com">kaka9887@naver.com</a></p>
  </div>

  <footer>
    본 개인정보처리방침은 네이버 블로그 통합 도우미 Chrome Extension의 데이터 처리 방식을 설명하기 위해 작성되었습니다.<br>
    최종 업데이트: 2026년 8월 29일
  </footer>
</main>
</body>
</html>
