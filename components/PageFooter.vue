<template>
  <div class="page-footer">
    <div class="container">
      <!-- find on -->
      <div class="find-on">
        <h5>{{ $t('PageFooter.text1') }}</h5>
        <div class="find-link">
          <a class="find-ain svgcolor1" href="#">
            <svg width="128" height="22" viewBox="0 0 128 22" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd" clip-rule="evenodd" d="M18.856 13.146c-.384.243-.836.273-1.18.08-.436-.247-.676-.824-.676-1.626V9.2c0-1.16-.458-1.984-1.225-2.207-1.299-.378-2.276 1.21-2.643 1.808l-2.291 3.713V7.975c-.026-1.044-.365-1.669-1.01-1.857-.426-.124-1.064-.074-1.683.873L3.014 15.23A9.048 9.048 0 0 1 1.971 11c0-4.963 3.979-9 8.87-9 4.89 0 8.869 4.037 8.869 9l.002.024v.025c.046.96-.266 1.726-.856 2.098zM21.681 11v-.025l-.001-.024C21.653 4.907 16.801 0 10.84 0 4.863 0 0 4.934 0 11c0 6.065 4.863 11 10.84 11a10.72 10.72 0 0 0 7.37-2.933 1.01 1.01 0 0 0-.257-1.642.976.976 0 0 0-1.083.175 8.769 8.769 0 0 1-6.03 2.4c-2.618 0-4.974-1.158-6.6-2.996l4.63-7.43V13c0 1.645.638 2.177 1.173 2.332.536.156 1.355.05 2.214-1.345l2.547-4.126c.081-.133.156-.248.225-.347V11.6c0 1.538.616 2.768 1.69 3.373.969.547 2.187.497 3.179-.128 1.202-.76 1.85-2.159 1.783-3.845zm15.092-3.758c.26.159.486.51.486.828 0 .51-.434.932-.92.932-.121 0-.242-.035-.347-.07-.572-.422-1.3-.704-2.064-.704-1.804 0-3.053 1.478-3.053 3.309 0 1.83 1.249 3.291 3.053 3.291.902 0 1.7-.37 2.307-.933a.937.937 0 0 1 .538-.176c.486 0 .867.387.867.88 0 .317-.19.599-.433.757-.868.74-2.047 1.232-3.262 1.232-2.775 0-5.03-2.288-5.03-5.104 0-2.816 2.254-5.104 5.03-5.104 1.041 0 2.03.317 2.828.862zm5.075 2.13c1.891 0 3.487 1.602 3.487 3.573 0 1.971-1.596 3.643-3.487 3.643-1.977 0-3.626-1.672-3.626-3.643 0-1.971 1.649-3.573 3.626-3.573zm-.017 5.456c.833 0 1.544-.792 1.544-1.866 0-1.073-.711-1.742-1.544-1.742-.902 0-1.649.651-1.649 1.742 0 1.074.747 1.866 1.649 1.866zm4.693.669v-5.034c0-.545.434-1.003.972-1.003s.989.458.989 1.003v5.034c0 .545-.451 1.003-.989 1.003s-.972-.458-.972-1.003zm-.155-7.938c0-.651.502-1.179 1.127-1.179.642 0 1.162.528 1.162 1.18 0 .633-.52 1.143-1.162 1.143-.625 0-1.127-.51-1.127-1.144zm5.873 5.21v2.728c0 .545-.451 1.003-.99 1.003-.537 0-.971-.458-.971-1.003v-5.263c0-.422.347-.774.764-.774.416 0 .746.352.746.774.798-.739 1.491-.862 2.15-.862 1.96 0 2.828 1.478 2.828 3.15v2.975c0 .545-.45 1.003-.988 1.003s-.972-.458-.972-1.003v-2.728c0-.863-.104-1.584-1.336-1.584-.867 0-1.232.721-1.232 1.584zm10.904 1.038a.639.639 0 0 1-.503-.246l-2.29-2.482v4.418c0 .545-.452 1.003-.99 1.003-.537 0-.971-.458-.971-1.003V6.75a.384.384 0 0 1 .365-.247c.173 0 .311.142.416.247l3.643 4.1c.104.124.243.194.312.194.07 0 .208-.07.312-.193l3.644-4.1c.104-.106.243-.248.416-.248s.312.106.365.247v8.747c0 .545-.434 1.003-.972 1.003s-.99-.458-.99-1.003v-4.418l-2.289 2.482c-.122.14-.278.246-.468.246zm9.43 1.021c.884 0 1.63-.792 1.63-1.866 0-1.073-.763-1.777-1.63-1.777-.868 0-1.562.721-1.562 1.777 0 1.039.694 1.866 1.561 1.866zm2.081.898l-.035-.23c-.381.757-1.596 1.092-2.377 1.092-1.84 0-3.192-1.672-3.192-3.643 0-1.971 1.388-3.573 3.296-3.573.33 0 1.423.088 2.273 1.091l.035-.229c0-.422.33-.774.746-.774s.763.352.763.774v5.492a.776.776 0 0 1-.764.774c-.416 0-.746-.352-.746-.774h.001zm6.949-4.541h-.208c-1.232.07-1.475.774-1.475 1.584v2.728c0 .545-.45 1.003-.989 1.003-.538 0-.971-.458-.971-1.003v-5.263c0-.422.346-.774.763-.774.417 0 .746.352.746.774.729-.686 1.319-.827 1.926-.862h.19c.47 0 .902.405.902.915 0 .475-.416.898-.884.898zm7.556 3.854c.087.141.139.3.139.475 0 .51-.469.986-.972.986-.347 0-.642-.264-.867-.546l-2.255-2.622v2.165c0 .545-.452 1.003-.99 1.003-.537 0-.971-.458-.971-1.003v-7.99c0-.546.434-1.004.971-1.004.538 0 .99.458.99 1.004v4.98l2.255-2.499c.225-.264.503-.528.85-.528.486 0 .937.458.937.968a.861.861 0 0 1-.122.458l-1.787 1.953 1.822 2.2zm3.844-3.819c-.538 0-1.406.282-1.406 1.109h2.828c0-.845-.902-1.109-1.423-1.109zm2.567 2.358H91.6c0 1.18 1.128 1.356 1.63 1.356.366 0 .886-.07 1.285-.247a.953.953 0 0 1 .503-.158c.433 0 .797.37.797.81 0 .299-.19.563-.433.703-.607.44-1.388.546-2.134.546-1.978 0-3.626-1.073-3.626-3.555 0-1.954 1.006-3.661 3.349-3.661 1.89 0 3.33 1.232 3.365 3.432a.776.776 0 0 1-.763.774zm5.457 3.01h-.538c-1.493 0-2.36-.651-2.36-2.992v-2.411h-.503c-.468 0-.884-.423-.884-.898 0-.51.416-.915.884-.915h.503V7.506c0-.545.434-1.003.972-1.003s.989.458.989 1.003v1.866h.815c.469 0 .885.405.885.915 0 .475-.416.898-.885.898h-.815v2.024c0 1.337.069 1.619.659 1.619h.278c.468 0 .867.387.867.88 0 .475-.399.88-.867.88zm9.499-9.346c.26.159.486.51.486.828 0 .51-.434.932-.92.932-.121 0-.243-.035-.347-.07-.573-.422-1.301-.704-2.064-.704-1.804 0-3.054 1.478-3.054 3.309 0 1.83 1.249 3.291 3.054 3.291.901 0 1.7-.37 2.307-.933a.938.938 0 0 1 .538-.176c.486 0 .867.387.867.88 0 .317-.191.599-.433.757-.868.74-2.048 1.232-3.262 1.232-2.776 0-5.031-2.288-5.031-5.104 0-2.816 2.255-5.104 5.031-5.104 1.041 0 2.03.317 2.828.862zm4.971 7.586c.885 0 1.63-.792 1.63-1.866 0-1.073-.763-1.777-1.63-1.777-.868 0-1.562.721-1.562 1.777 0 1.039.694 1.866 1.562 1.866zm2.081.898l-.034-.23c-.382.757-1.596 1.092-2.377 1.092-1.839 0-3.192-1.672-3.192-3.643 0-1.971 1.388-3.573 3.296-3.573.33 0 1.423.088 2.273 1.091l.034-.229c0-.422.33-.774.747-.774.416 0 .763.352.763.774v5.492a.776.776 0 0 1-.763.774c-.417 0-.747-.352-.747-.774zm6.897-.898c.868 0 1.561-.827 1.561-1.866 0-1.056-.693-1.777-1.561-1.777-.867 0-1.631.704-1.631 1.777 0 1.074.747 1.866 1.631 1.866zm-1.631 1.18v2.498c0 .546-.451 1.004-.989 1.004-.537 0-.971-.458-.971-1.004v-8.272c0-.422.347-.774.764-.774.416 0 .746.352.746.845.728-.757 1.63-.933 2.307-.933 1.908 0 3.296 1.602 3.296 3.573 0 1.971-1.353 3.643-3.192 3.643-.572 0-1.423-.176-1.961-.58z" fill="var(--color-1, white)">
              </path>
            </svg>
          </a>
          <a class="find-ain svgcolor2" href="#">
            <svg width="95" height="25" viewBox="0 0 95 25" xmlns="http://www.w3.org/2000/svg">
              <g clip-path="url(#clip0-gekko)">
                <path d="M39.269 9.817c-.258-1.003-.91-1.737-2.183-1.737-1.88 0-2.666 1.65-2.666 3.325 0 1.675.786 3.326 2.666 3.326 1.364 0 2.112-1.015 2.234-2.286h1.498c-.123 2.09-1.608 3.532-3.73 3.532-2.628 0-4.2-2.079-4.2-4.573s1.567-4.576 4.195-4.576c1.977.012 3.536 1.1 3.72 2.983l-1.534.006zM41.725 12.599c0-1.932 1.166-3.325 3.205-3.325s3.205 1.393 3.205 3.325c0 1.931-1.166 3.338-3.205 3.338s-3.205-1.394-3.205-3.338zm5.01 0c0-1.087-.552-2.225-1.805-2.225s-1.805 1.137-1.805 2.225c0 1.087.552 2.237 1.805 2.237s1.805-1.137 1.805-2.237zM49.339 7.036h1.4v1.32h-1.4v-1.32zm0 2.41h1.4v6.32h-1.4v-6.32zM52.262 9.445h1.326v.93l.025.024a2.27 2.27 0 0 1 1.977-1.126c1.376 0 2.247.734 2.247 2.15v4.342h-1.4v-3.973c-.024-.99-.417-1.418-1.24-1.418-.933 0-1.535.733-1.535 1.662v3.73h-1.4v-6.32zM67.158 15.766h-.982l-.233-1.027c-.819.93-1.572 1.234-2.639 1.234-2.626.002-4.202-2.08-4.202-4.572s1.576-4.573 4.2-4.573c1.911 0 3.525 1.014 3.758 2.983H65.56c-.147-1.15-1.153-1.736-2.258-1.736-1.88 0-2.666 1.65-2.666 3.325 0 1.674.786 3.325 2.666 3.325 1.57.025 2.43-.916 2.456-2.396h-2.334v-1.16h3.73l.003 4.597zM69.725 12.965c0 .991.54 1.871 1.707 1.871.81 0 1.302-.354 1.546-1.051h1.328c-.307 1.381-1.486 2.152-2.874 2.152-1.989 0-3.107-1.382-3.107-3.326 0-1.797 1.183-3.337 3.07-3.337 2.002 0 3.23 1.797 2.997 3.691h-4.667zm3.267-.916c-.05-.88-.651-1.675-1.597-1.675-.97 0-1.632.733-1.67 1.675h3.267zM79.747 11.56c-.111-.77-.676-1.186-1.45-1.186-.727 0-1.743.379-1.743 2.298 0 1.051.466 2.164 1.682 2.164.81 0 1.375-.537 1.511-1.442h1.4c-.258 1.638-1.274 2.543-2.911 2.543-1.99 0-3.082-1.407-3.082-3.265 0-1.907 1.044-3.398 3.131-3.398 1.474 0 2.73.734 2.862 2.286h-1.4zM82.33 7.036h1.4V12l2.53-2.555h1.719l-2.432 2.322 2.665 3.999h-1.71l-1.94-3.07-.836.808v2.264H82.33V7.036zM88.59 12.599c0-1.932 1.166-3.325 3.204-3.325 2.039 0 3.206 1.393 3.206 3.325 0 1.931-1.167 3.338-3.206 3.338-2.038 0-3.205-1.394-3.205-3.338zm5.01 0c0-1.087-.553-2.225-1.806-2.225-1.252 0-1.805 1.137-1.805 2.225 0 1.087.553 2.237 1.805 2.237 1.253 0 1.806-1.137 1.806-2.237z" fill="var(--color-1, white)">
                </path>
                <path d="M25.109 12.443a12.46 12.46 0 0 1-2.085 6.952 12.541 12.541 0 0 1-5.614 4.628 12.606 12.606 0 0 1-7.25.743 12.572 12.572 0 0 1-6.443-3.392A12.482 12.482 0 0 1 .253 14.99a12.446 12.446 0 0 1 .682-7.225 12.51 12.51 0 0 1 4.6-5.629 12.594 12.594 0 0 1 15.858 1.485 12.47 12.47 0 0 1 3.716 8.822z" fill="var(--color-5, #CECECE)">
                </path>
                <path d="M24.167 12.447c.01 2.286-.66 4.524-1.928 6.431a11.6 11.6 0 0 1-5.191 4.28 11.66 11.66 0 0 1-6.706.689 11.627 11.627 0 0 1-5.959-3.137 11.544 11.544 0 0 1-3.204-5.904 11.511 11.511 0 0 1 .63-6.682 11.57 11.57 0 0 1 4.253-5.206A11.647 11.647 0 0 1 20.73 4.29a11.534 11.534 0 0 1 3.438 8.157z" fill="var(--color-6, #FDFDFD)">
                </path>
                <path d="M12.768 1.69a6.412 6.412 0 0 1 2.231 0 6.812 6.812 0 0 1 2.132.71c.662.363 1.235.855 1.804 1.316.57.46 1.136.933 1.676 1.449a8.464 8.464 0 0 1 1.429 1.72c.41.63.745 1.303 1 2.009.485 1.418.654 2.946.412 4.403h-.072c-.243-1.445-.572-2.821-1.092-4.13a16.08 16.08 0 0 0-.859-1.925 18.9 18.9 0 0 0-1.13-1.805 6.563 6.563 0 0 0-1.513-1.522c-.59-.418-1.268-.69-1.923-.946-.656-.258-1.307-.524-1.99-.72a25.323 25.323 0 0 0-2.106-.484l.001-.075z" fill="var(--color-1, white)">
                </path>
                <path d="M18.444 8.367c-.843-.242-1.716-.586-2.6-.934-.051-.221-.248-.497-.646-.833-.577-.499-1.662-.486-2.6-.265-1.036-.243-2.058-.329-3.04-.09-8.028 2.201-3.476 7.573-6.423 12.972.42.886 4.94 6.054 11.48 4.667 0 0-2.237-5.351 2.811-7.92 4.095-2.091 7.054-5.96 1.018-7.597z" fill="var(--color-3, #D5D5D5)">
                </path>
                <path d="M19.435 11.882a.483.483 0 0 1-.579.479.487.487 0 0 1-.358-.659.486.486 0 0 1 .937.18z" fill="var(--color-1, white)">
                </path>
                <path d="M12.598 6.331c.585.042 2.7.725 3.245 1.098-.454-1.313-1.985-1.488-3.245-1.098z" fill="var(--color-2, #959595)">
                </path>
                <path d="M13.154 9.652c0 .443-.13.875-.377 1.243a2.243 2.243 0 0 1-2.305.95 2.248 2.248 0 0 1-1.15-.61 2.232 2.232 0 0 1-.487-2.437 2.252 2.252 0 0 1 4.149-.001c.112.271.17.562.17.855z" fill="var(--color-1, white)">
                </path>
                <path d="M12.489 9.672a1.567 1.567 0 0 1-.975 1.453 1.586 1.586 0 0 1-1.721-.34A1.57 1.57 0 0 1 10.909 8.1c.42 0 .82.166 1.117.46.296.295.463.695.463 1.112z" fill="var(--color-4, #58595B)">
                </path>
                <path d="M21.254 12.868c-1.82 1.276-3.888 2.244-6.823 2.244-1.374 0-1.652-1.45-2.56-.74-.468.367-2.12 1.19-3.431 1.127-1.311-.063-3.436-.828-4.029-3.614-.234 2.786-.354 4.838-1.405 7.19 2.092 3.336 7.081 5.909 11.61 4.8-.487-3.383 2.482-6.695 4.155-8.39.637-.643 1.847-1.69 2.483-2.62v.003z" fill="var(--color-3, #D5D5D5)">
                </path>
                <path d="M21.183 12.95c-.565.514-1.237.893-1.921 1.228-.693.327-1.415.59-2.157.782-.742.19-1.516.335-2.3.264-.784-.07-1.586-.336-2.105-.92l.024-.029c.637.411 1.372.556 2.104.577a9.918 9.918 0 0 0 2.21-.181 12.087 12.087 0 0 0 2.148-.661c.694-.286 1.38-.616 1.972-1.087l.025.028z" fill="var(--color-4, #58595B)">
                </path>
              </g>
              <defs>
                <clipPath id="clip0-gekko">
                  <path fill="var(--color-1, white)" d="M0 0h95v25H0z">
                  </path>
                </clipPath>
              </defs>
            </svg>
          </a>
          <a class="find-ain svgcolor1" href="#">
            <svg width="126" height="25" viewBox="0 0 126 25" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd" clip-rule="evenodd" d="M32.533 18.1c-2.756 0-4.794-2.13-4.794-4.745s2.038-4.797 4.811-4.797c1.757 0 2.845.641 3.706 1.576l-1.317 1.403c-.65-.675-1.334-1.143-2.406-1.143-1.545 0-2.669 1.316-2.669 2.926 0 1.645 1.14 2.962 2.774 2.962 1.002 0 1.739-.468 2.406-1.143l1.282 1.246c-.913 1.005-1.984 1.715-3.793 1.715zm7.824 0h-2.123V8.576h2.124v2.233c.58-1.367 1.65-2.303 3.283-2.233v2.217h-.123c-1.86 0-3.16 1.194-3.16 3.619V18.1zm14.406-9.541l-4.695 12.105h-2.155l1.027-2.561-4.022-9.544h2.265l2.743 7.049 2.636-7.05h2.2zm6.268 1.817c-1.44 0-2.704 1.16-2.704 2.944s1.264 2.944 2.704 2.944c1.457 0 2.651-1.125 2.651-2.944 0-1.801-1.212-2.944-2.651-2.944zm.491 7.706c-1.527 0-2.493-.762-3.143-1.61v4.191h-2.125V8.56h2.125v1.714c.685-.952 1.651-1.714 3.143-1.714 2.195 0 4.32 1.714 4.32 4.762 0 3.048-2.107 4.762-4.32 4.762zM70.5 10.55v4.484c0 .813.42 1.142 1.141 1.142h.834v1.871H71.02c-1.546-.004-2.645-.682-2.645-2.684V10.55h-1.18v-1.8h1.18V6.24H70.5V8.75h1.975v1.799h-1.975zm8.695-.156c-1.704 0-2.793 1.316-2.793 2.926 0 1.628 1.177 2.962 2.828 2.962 1.72 0 2.809-1.317 2.809-2.927 0-1.628-1.177-2.961-2.844-2.961zm0 7.706c-2.828 0-4.918-2.13-4.918-4.745 0-2.632 2.108-4.797 4.953-4.797 2.844 0 4.934 2.13 4.934 4.762 0 2.616-2.108 4.78-4.97 4.78zm8.857-1.921v1.056a.117.117 0 0 1-.061.105l-.927.528a.122.122 0 0 1-.123 0l-.93-.528a.122.122 0 0 1-.061-.105v-1.056c0-.043.025-.083.062-.106l.929-.528a.121.121 0 0 1 .123 0l.927.528a.123.123 0 0 1 .062.106h-.001zm16.425-5.785c-1.704 0-2.793 1.316-2.793 2.926 0 1.628 1.177 2.962 2.828 2.962 1.72 0 2.808-1.317 2.808-2.927 0-1.628-1.176-2.961-2.843-2.961zm0 7.706c-2.828 0-4.918-2.13-4.918-4.745 0-2.632 2.107-4.797 4.953-4.797 2.844 0 4.934 2.13 4.934 4.762 0 2.616-2.108 4.78-4.969 4.78zm-9.956-.01c-2.756-.053-4.751-2.221-4.7-4.836.05-2.614 2.13-4.757 4.903-4.704 1.756.033 2.832.694 3.674 1.645l-1.344 1.378c-.636-.688-1.312-1.168-2.383-1.189-1.545-.029-2.695 1.265-2.726 2.875-.032 1.646 1.084 2.984 2.716 3.014 1.002.02 1.748-.434 2.428-1.097l1.258 1.271c-.933.987-2.017 1.677-3.825 1.643h-.001zm27.553-9.531c2.02 0 3.248 1.263 3.248 3.497V18.1h-2.124v-5.403c0-1.454-.685-2.234-1.879-2.234-1.158 0-1.984.796-1.984 2.269V18.1h-2.124v-5.42c0-1.42-.703-2.217-1.879-2.217-1.177 0-1.985.866-1.985 2.287v5.35h-2.125V8.559h2.125v1.576c.597-.814 1.406-1.576 2.827-1.576 1.335 0 2.265.64 2.757 1.61.756-.97 1.738-1.61 3.143-1.61zM0 6.687v11.905l10.4 5.953 10.397-5.953V6.687L10.4.735 0 6.687zM.916 18.07V7.212L10.4 1.78l9.485 5.432V18.07L10.4 23.5.916 18.07z" fill="var(--color-1, white)">
              </path>
              <path fill-rule="evenodd" clip-rule="evenodd" d="M14.475 5.875H6.304l-.947 4.13H15.46l-.985-4.13zM7.754 15.69v-2.745l-2.422-1.526-2.739 2.02 3.734 6.437h1.491l1.764-1.628v-.819l-1.828-1.74z" fill="var(--color-1, white)">
              </path>
              <path fill-rule="evenodd" clip-rule="evenodd" d="M13.054 10.629H7.761l.892 2.307-.271 2.586h2.016l2.036-.01-.254-2.576.874-2.307z" fill="var(--color-1, white)">
              </path>
              <path fill-rule="evenodd" clip-rule="evenodd" d="M15.474 11.4l-2.392 1.545v2.745l-1.83 1.74v.818l1.764 1.61h1.473l3.716-6.42-2.73-2.037z" fill="var(--color-1, white)">
              </path>
            </svg>
          </a>
        </div>
      </div>
      <!-- link list -->
      <ul class="vlistbox">
        <li class="vlistitem">
          <p class="vping">
            {{ $t('PageFooter.text2') }}
          </p>
          <ul class="vainitemcell">
      
            <li class="vw100item">
              <a class="aintext" tabindex="0" aria-disabled="false" href="https://github.com/sellToken?tab=repositories" role="link" target="_blank" rel="noreferrer">
                <span class="atext">
                  <div class="gintext">
                    Github
                  </div>
                </span>
              </a>
            </li>
          </ul>
        </li>
        <li class="vlistitem">
          <p class="vping">
            {{ $t('PageFooter.text8') }}
          </p>
          <ul class="vainitemcell">
            <li class="vw100item">
              <a class="aintext" tabindex="0" aria-disabled="false" role="link" href="https://www.selltoken.org/Whitepaper.pdf">
                <span class="atext">
                  <div class="gintext">
                    {{ $t('PageFooter.text6') }}
                  </div>
                </span>
              </a>
            </li>
            <li class="vw100item">
             <a class="aintext" tabindex="0" aria-disabled="false" role="link" href="https://www.selltoken.org/WhitepaperCn.pdf">
                <span class="atext">
                  <div class="gintext">
                    {{ $t('PageFooter.text7') }}
                  </div>
                </span>
              </a>
            </li>
          </ul>
        </li>
        <li class="vlistitem">
          <p class="vping">
            {{ $t('PageFooter.text3') }}
          </p>
          <ul class="vainitemcell">
            <li class="vw100item">
              <a class="aintext" tabindex="0" aria-disabled="false" role="link" href="#">
                <span class="atext">
                  <div class="gintext">
                    {{ $t('PageFooter.text4') }}
                  </div>
                </span>
              </a>
            </li>
            <li class="vw100item">
              <a class="aintext" tabindex="0" aria-disabled="false" role="link" href="https://bscscan.com/address/0xa645995e9801f2ca6e2361edf4c2a138362bade4#code">
                <span class="atext">
                  <div class="gintext">
                    {{ $t('PageFooter.text5') }}
                  </div>
                </span>
              </a>
            </li>
            <li class="vw100item">
             
            </li>
            <li class="vw100item">
              
            </li>
          </ul>
        </li>
        <li class="vlistitem">
          <p class="vping">
            {{ $t('PageFooter.text9') }}
          </p>
          <ul class="vainitemcell">
            <li class="vw100item">
              <a class="aintext" tabindex="0" aria-disabled="false" href="https://twitter.com/TrustTheTrident" role="link" target="_blank" rel="noreferrer">
                <span class="atext">
                  <div class="gintext">
                    <svg fill="none" height="12" viewBox="0 0 14 12" width="14" xmlns="http://www.w3.org/2000/svg">
                      <path clip-rule="evenodd" d="M12.575 3.415c0-.132-.002-.262-.008-.39A5.9 5.9 0 0 0 14 1.485a5.562 5.562 0 0 1-1.65.452 2.937 2.937 0 0 0 1.262-1.65A5.464 5.464 0 0 1 11.79.99 2.862 2.862 0 0 0 9.694 0C8.107-.025 6.822 1.314 6.822 2.994c0 .239.025.47.073.695C4.506 3.535 2.391 2.292.975.417c-.246.449-.39.974-.39 1.537 0 1.063.507 2.008 1.278 2.567a2.765 2.765 0 0 1-1.3-.398v.039c0 1.486.99 2.732 2.303 3.023a2.707 2.707 0 0 1-1.297.044c.364 1.219 1.427 2.11 2.681 2.138A5.544 5.544 0 0 1 0 10.621 7.742 7.742 0 0 0 4.404 12c5.284 0 8.17-4.596 8.17-8.585z" fill="#82899a" fill-rule="evenodd">
                      </path>
                    </svg>
                    {{ $t('PageFooter.text10') }}
                  </div>
                </span>
              </a>
            </li>
            <li class="vw100item">
              <a class="aintext" tabindex="0" aria-disabled="false" href="https://t.me/TrustTheTrident" role="link" target="_blank" rel="noreferrer">
                <span class="atext">
                  <div class="gintext">
                    <svg fill="none" height="13" viewBox="0 0 15 13" width="15" xmlns="http://www.w3.org/2000/svg">
                      <path clip-rule="evenodd" d="M11.49 12.857a.72.72 0 0 0 .692.094.746.746 0 0 0 .452-.546C13.178 9.75 14.494 3.03 14.99.616a.52.52 0 0 0-.162-.492.485.485 0 0 0-.498-.091C11.709 1.04 3.638 4.19.339 5.46A.538.538 0 0 0 0 5.98c.008.23.156.43.37.496 1.48.46 3.422 1.1 3.422 1.1s.908 2.85 1.38 4.3c.06.182.197.325.378.375a.527.527 0 0 0 .506-.135l1.935-1.9s2.233 1.702 3.499 2.64zm-6.881-5.64l1.05 3.6.232-2.28 6.366-5.971a.186.186 0 0 0 .02-.245.173.173 0 0 0-.234-.042L4.609 7.216z" fill="#82899a" fill-rule="evenodd">
                      </path>
                    </svg>
                    {{ $t('PageFooter.text11') }}
                  </div>
                </span>
              </a>
            </li>
            <li class="vw100item">
              <a class="aintext" tabindex="0" aria-disabled="false" href="https://t.me/selltokenGroup" role="link" target="_blank" rel="noreferrer">
                <span class="atext">
                  <div class="gintext">
                    <svg fill="none" height="13" viewBox="0 0 15 13" width="15" xmlns="http://www.w3.org/2000/svg">
                      <path clip-rule="evenodd" d="M11.49 12.857a.72.72 0 0 0 .692.094.746.746 0 0 0 .452-.546C13.178 9.75 14.494 3.03 14.99.616a.52.52 0 0 0-.162-.492.485.485 0 0 0-.498-.091C11.709 1.04 3.638 4.19.339 5.46A.538.538 0 0 0 0 5.98c.008.23.156.43.37.496 1.48.46 3.422 1.1 3.422 1.1s.908 2.85 1.38 4.3c.06.182.197.325.378.375a.527.527 0 0 0 .506-.135l1.935-1.9s2.233 1.702 3.499 2.64zm-6.881-5.64l1.05 3.6.232-2.28 6.366-5.971a.186.186 0 0 0 .02-.245.173.173 0 0 0-.234-.042L4.609 7.216z" fill="#82899a" fill-rule="evenodd">
                      </path>
                    </svg>
                    {{ $t('PageFooter.text12') }}
                  </div>
                </span>
              </a>
            </li>
          </ul>
        </li>
        <li class="vlistitem">
          <p class="vping">
            {{ $t('PageFooter.text13') }}
          </p>
          <ul class="vainitemcell">
            <li class="vw100item">
              <a class="aintext" tabindex="0" aria-disabled="false" role="link" href="https://t.me/TrustTheTrident">
                <span class="atext">
                  <div class="gintext">
                    {{ $t('PageFooter.text14') }}
                  </div>
                </span>
              </a>
            </li>
          </ul>
        </li>
      </ul>
      <!-- footer -->
      <div class="footer-copylink">
        <div class="lt-logo">
          <a class="#">
            <img src="~/static/images/logo.png" height="52">
          </a>
        </div>
        <p class="f-text">
          <span>
            © 2023 SellToken All rights reserved | selltoken.org | selltoken.net | info@selltoken.org
          </span>
        </p>
        <ul class="vrbox">
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PageFooter'
}
</script>

<style lang="scss" scoped>
.page-footer {
  padding: 30px 0 100px;
  .find-on {
    width: 100%;
    display: flex;
    flex-direction: column;
    border-bottom: 2px solid #F2F5FA;
    padding-bottom: 20px;
    h5 {
      font-size: 16px;
      font-weight: normal;
    }
    .find-link {
      display: flex;
      flex-wrap: wrap;
      .find-ain {
        color: #1f2226;
        opacity: 0.5;
        margin-top: 24px;
        padding-right: 24px;
        justify-content: flex-start;
        transition-duration: 250ms;
        transition-property: opacity;
        transition-timing-function: linear;
        min-width: 160px;
        &.svgcolor1,
        &.svgcolor2 {
          --color-1: currentColor;
          --color-2: #959595;
          --color-3: #D5D5D5;
          --color-4: #58595B;
          --color-5: #CECECE;
          --color-6: #FDFDFD;
        }
        &:hover {
          opacity: 1;
          &.svgcolor2 {
            --color-1: currentColor;
            --color-2: #009345;
            --color-3: #8BC53F;
            --color-4: #58595B;
            --color-5: #8DC63F;
            --color-6: #F9E988;
          }
        }
      }
    }
  }
}
.vlistbox {
  gap: 15px;
  width: 100%;
  margin: 0;
  display: flex;
  padding: 30px 0 0;
  list-style: none;
  flex-direction: row;
  justify-content: flex-start;
  .vlistitem {
    width: calc(100% / 5);
    box-sizing: border-box;
  }
  .vping {
    display: flex;
    align-items: center;
    flex-direction: row;
    font-size: 16px;
    color: #1f2226;
    font-weight: 400;
    line-height: 1.2;
  }
  .vainitemcell {
    margin: 0;
    display: flex;
    padding: 0;
    list-style: none;
    margin-top: 16px;
    align-items: flex-start;
    flex-direction: column;
    .vw100item {
      width: 100%;
      height: 38px;
    }
  }
  .aintext {
    color: rgba(31, 34, 38, 0.5);
    width: auto;
    padding: 10px 0px;
    text-transform: inherit;
    justify-content: flex-start;
    transition-duration: 300ms;
    transition-property: color;
    transition-timing-function: linear;
    font-size: 14px;
    .atext {
      width: 100%;
      display: inherit;
      align-items: inherit;
      justify-content: inherit;
    }
    .gintext {
      gap: 15px;
      display: flex;
      align-items: center;
    }
    &:hover {
      color: rgba(31, 34, 38, 1);
    }
  }
}
.footer-copylink {
  display: flex;
  padding: 24px 0px;
  border-top: 2px solid #F2F5FA;
  align-items: center;
  flex-direction: row;
  .lt-logo {
    display: flex;
    width: 25%;
    margin-right: 0;
    img {
      height: 52px;
    }
  }
  .f-text {
    color: rgba(31, 34, 38, 0.5);
    flex-grow: 1;
    font-size: 14px;
    a {
      color: inherit;
      transition: color 0.2s;
      text-decoration: none;
      cursor: pointer;
      &:hover {
        color: #356DF3;
      }
    }
  }
  .vrbox {
    margin: 0;
    display: flex;
    padding: 0;
    flex-wrap: wrap;
    list-style: none;
    align-items: center;
    flex-direction: row;
    justify-content: flex-end;
  }
  .vrt {
    color: rgba(31, 34, 38, 0.4);
    padding: 8px 0px;
    font-size: 15px;
    transition: color 0.2s;
    text-transform: inherit;
    &:hover {
      color: #356DF3;
    }
  }
}
@media screen and (max-width: 750px) {
  .vlistbox {
    flex-wrap: wrap;
    gap: 0;
    .vlistitem {
      width: 50%;
    }
  }
  .footer-copylink {
    flex-direction: column;
    .lt-logo {
      width: 100%;
      @include flexBox;
    }
    .f-text {
      text-align: center;
      padding: 10px 0;
    }
  }
}
</style>
