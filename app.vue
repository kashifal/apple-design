<template>
  <div>
    <Navbar />
    <div>
      <div class="">
        <div class="mx-auto max-w-[85rem] justify-between gap-3 px-4 py-20">
          <Gallery />

          <div class="pt-12">
            <div
              class="flex flex-col items-center justify-between gap-8 border-b pb-6 text-center sm:flex-row sm:gap-3 sm:text-left"
            >
              <div class="flex flex-col items-center sm:items-start">
                <h1
                  class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-2xl font-semibold text-black"
                >
                  IPad Pro Special Black Edition
                </h1>

                <div class="flex items-center gap-1 pt-4">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-5 w-5 text-[#E2B704]"
                    width="1em"
                    height="1em"
                    viewBox="0 0 24 24"
                  >
                    <path
                      fill="currentColor"
                      d="m12 17.27l4.15 2.51c.76.46 1.69-.22 1.49-1.08l-1.1-4.72l3.67-3.18c.67-.58.31-1.68-.57-1.75l-4.83-.41l-1.89-4.46c-.34-.81-1.5-.81-1.84 0L9.19 8.63l-4.83.41c-.88.07-1.24 1.17-.57 1.75l3.67 3.18l-1.1 4.72c-.2.86.73 1.54 1.49 1.08z"
                    />
                  </svg>

                  <h1
                    class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-xl font-semibold"
                  >
                    4.8
                    <span class="text-[16px] font-normal text-gray-600">
                      (1624 Bewertungen)
                    </span>
                  </h1>
                </div>
              </div>

              <div class="flex items-start">
                <button
                  class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] rounded-lg px-10 py-2 font-medium text-white shadow-xl hover:border hover:border-[#5A9FFA]"
                  style="
                    background: linear-gradient(to right, #5a9ffa, #3373ee);
                  "
                >
                  Jetzt Voten!
                </button>
                <div class="-ml-2 -mt-1">
                  <span class="relative flex h-3 w-3"
                    ><span
                      class="absolute inline-flex h-full w-full animate-ping rounded-full bg-[#3373EE] opacity-80"
                    ></span
                    ><span
                      class="relative inline-flex h-3 w-3 rounded-full bg-[#3373EE]"
                    ></span
                  ></span>
                </div>
              </div>
            </div>

            <h3
              class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] py-5 text-gray-600"
            >
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel
              deserunt quasi delectus dolorum quam? Est rem vero rerum dolores
              omnis quasi temporibus nihil facere tempora. Dolores aut odio
              rerum at!
            </h3>

            <div class="mt-12">
              <ul class="grid w-full gap-4 sm:grid-cols-2">
                <li>
                  <input
                    type="radio"
                    id="hosting-small"
                    name="hosting"
                    value="hosting-small"
                    class="peer hidden"
                    required
                  />
                  <label
                    for="hosting-small"
                    class="inline-flex w-full cursor-pointer items-center justify-between rounded-lg border-2 border-[#F3F3F3] bg-white p-6 hover:bg-gray-100 hover:text-gray-600 peer-checked:bg-gray-100 peer-checked:border-blue-600 peer-checked:text-white"
                  >
                    <div class="block w-full text-center">
                      <div
                        class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-2xl text-[#151515]"
                      >
                        Spieler
                      </div>
                      <div
                        class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] pt-2 text-4xl font-semibold text-black"
                      >
                        100/100
                      </div>
                    </div>
                  </label>
                </li>
                <li>
                  <input
                    type="radio"
                    id="hosting-big"
                    name="hosting"
                    value="hosting-big"
                    class="peer hidden"
                  />
                  <label
                    for="hosting-big"
                    class="inline-flex w-full cursor-pointer items-center justify-between rounded-lg border-2 border-[#F3F3F3] bg-white p-6 hover:bg-gray-100 hover:text-gray-600 peer-checked:bg-gray-100 peer-checked:border-blue-600 peer-checked:text-white"
                  >
                    <div class="block w-full text-center">
                      <div
                        class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-2xl text-[#151515]"
                      >
                        Registriert
                      </div>
                      <div
                        class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] pt-2 text-4xl font-semibold text-black"
                      >
                        1.000+
                      </div>
                    </div>
                  </label>
                </li>

                <li>
                  <input
                    type="radio"
                    id="hosting-large"
                    name="hosting"
                    value="hosting-large"
                    class="peer hidden"
                    required
                  />
                  <label
                    for="hosting-large"
                    class="inline-flex w-full cursor-pointer items-center justify-between rounded-lg border-2 border-[#F3F3F3] bg-white p-6 hover:bg-gray-100 hover:text-gray-600 peer-checked:bg-gray-100 peer-checked:border-blue-600 peer-checked:text-white"
                  >
                    <div class="block w-full text-center">
                      <div
                        class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-2xl text-[#151515]"
                      >
                        Spielzeit
                      </div>
                      <div
                        class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] pt-2 text-4xl font-semibold text-black"
                      >
                        100.000h
                      </div>
                    </div>
                  </label>
                </li>

                <li>
                  <input
                    type="radio"
                    id="hosting-xl"
                    name="hosting"
                    value="hosting-xl"
                    class="peer hidden"
                    required
                  />
                  <label
                    for="hosting-xl"
                    class="inline-flex w-full cursor-pointer items-center justify-between rounded-lg border-2 border-[#F3F3F3] bg-white p-6 hover:bg-gray-100 hover:text-gray-600 peer-checked:bg-gray-100 peer-checked:border-blue-600 peer-checked:text-white"
                  >
                    <div class="block w-full text-center">
                      <div
                        class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-2xl text-[#151515]"
                      >
                        Votes
                      </div>
                      <div
                        class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] pt-2 text-4xl font-semibold text-black"
                      >
                        1.000.000
                      </div>
                    </div>
                  </label>
                </li>
              </ul>
            </div>

            <div class="py-12">
              <h1
                class="font-[SF Pro Display,SF Pro Icons,Helvetica Neue,Helvetica,Arial,sans-serif] text-xl font-semibold"
              >
                Bewertungen
              </h1>
              <Comments />
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>
