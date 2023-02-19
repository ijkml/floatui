---
title: Pricing Section with two plans
category: Marketing
paid: true
isActive: true
ltr: {"vue":{"vueCss":[],"vueTail":[]},"react":{"jsxCss":[],"jsxTail":[{"code":"export default () => {\n\n    const plans = [\n        {\n            name: \"Enterprise\",\n            desc: \"Lorem ipsum dolor sit amet, consectetur adipiscing elit.\",\n            price: 32,\n            isMostPop: true,\n            features: [\n                \"Curabitur faucibus\",\n                \"massa ut pretium maximus\",\n                \"Sed posuere nisi\",\n                \"Pellentesque eu nibh et neque\",\n                \"Suspendisse a leo\",\n                \"Praesent quis venenatis ipsum\",\n                \"Duis non diam vel tortor\",\n            ],\n        },\n        {\n            name: \"Startup\",\n            desc: \"Lorem ipsum dolor sit amet, consectetur adipiscing elit.\",\n            price: 12,\n            isMostPop: false,\n            features: [\n                \"Curabitur faucibus\",\n                \"massa ut pretium maximus\",\n                \"Sed posuere nisi\",\n                \"Pellentesque eu nibh et neque\",\n                \"Suspendisse a leo\",\n                \"Praesent quis venenatis ipsum\",\n                \"Duis non diam vel tortor\",\n            ],\n        },\n    ];\n\n    return (\n        <section className='relative py-14'>\n            <div className=\"absolute top-0 w-full h-[521px]\" style={{ background: \"linear-gradient(152.92deg, rgba(192, 132, 252, 0.2) 4.54%, rgba(232, 121, 249, 0.17) 34.2%, rgba(192, 132, 252, 0.1) 77.55%)\" }}></div>\n            <div className=\"max-w-screen-xl mx-auto text-gray-600 sm:px-4 md:px-8\">\n                <div className='relative max-w-xl mx-auto space-y-3 px-4 sm:text-center sm:px-0'>\n                    <h3 className=\"text-indigo-600 font-semibold\">\n                        Pricing\n                    </h3>\n                    <p className='text-gray-800 text-3xl font-semibold sm:text-4xl'>\n                        Pay as you grow\n                    </p>\n                    <div className='max-w-xl'>\n                        <p>\n                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam efficitur consequat nunc.\n                        </p>\n                    </div>\n                </div>\n                <div className='mt-16 justify-center sm:flex'>\n                    {\n                        plans.map((item, idx) => (\n                            <div key={idx} className={`relative flex-1 flex items-stretch flex-col mt-6 sm:mt-0 sm:rounded-xl sm:max-w-md ${item.isMostPop ? \"bg-white shadow-lg sm:border\" : \"\"}`}>\n                                <div className=\"p-4 py-8 space-y-4 border-b md:p-8\">\n                                    <span className='text-indigo-600 font-medium'>\n                                        {item.name}\n                                    </span>\n                                    <div className='text-gray-800 text-3xl font-semibold'>\n                                        ${item.price} <span className=\"text-xl text-gray-600 font-normal\">/mo</span>\n                                    </div>\n                                    <p>\n                                        {item.desc}\n                                    </p>\n                                    <button className='px-3 py-3 rounded-lg w-full font-semibold text-sm duration-150 text-white bg-indigo-600 hover:bg-indigo-500 active:bg-indigo-700'>\n                                        Get Started\n                                    </button>\n                                </div>\n                                <ul className='p-4 py-8 space-y-3 md:p-8'>\n                                    <li className=\"pb-2 text-gray-800 font-medium\">\n                                        <p>Features</p>\n                                    </li>\n                                    {\n                                        item.features.map((featureItem, idx) => (\n                                            <li key={idx} className='flex items-center gap-5'>\n                                                <svg\n                                                    xmlns='http://www.w3.org/2000/svg'\n                                                    className='h-5 w-5 text-indigo-600'\n                                                    viewBox='0 0 20 20'\n                                                    fill='currentColor'>\n                                                    <path\n                                                        fill-rule='evenodd'\n                                                        d='M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z'\n                                                        clip-rule='evenodd'></path>\n                                                </svg>\n                                                {featureItem}\n                                            </li>\n                                        ))\n                                    }\n                                </ul>\n                            </div>\n                        ))\n                    }\n                </div>\n            </div>\n        </section>\n    );\n};\n","label":"App.jsx"}]},"preview":"function App() {\n  const plans = [{\n    name: \"Enterprise\",\n    desc: \"Lorem ipsum dolor sit amet, consectetur adipiscing elit.\",\n    price: 32,\n    isMostPop: true,\n    features: [\"Curabitur faucibus\", \"massa ut pretium maximus\", \"Sed posuere nisi\", \"Pellentesque eu nibh et neque\", \"Suspendisse a leo\", \"Praesent quis venenatis ipsum\", \"Duis non diam vel tortor\"]\n  }, {\n    name: \"Startup\",\n    desc: \"Lorem ipsum dolor sit amet, consectetur adipiscing elit.\",\n    price: 12,\n    isMostPop: false,\n    features: [\"Curabitur faucibus\", \"massa ut pretium maximus\", \"Sed posuere nisi\", \"Pellentesque eu nibh et neque\", \"Suspendisse a leo\", \"Praesent quis venenatis ipsum\", \"Duis non diam vel tortor\"]\n  }];\n  return /*#__PURE__*/React.createElement(\"section\", {\n    className: \"relative py-14\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"absolute top-0 w-full h-[521px]\",\n    style: {\n      background: \"linear-gradient(152.92deg, rgba(192, 132, 252, 0.2) 4.54%, rgba(232, 121, 249, 0.17) 34.2%, rgba(192, 132, 252, 0.1) 77.55%)\"\n    }\n  }), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"max-w-screen-xl mx-auto text-gray-600 sm:px-4 md:px-8\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"relative max-w-xl mx-auto space-y-3 px-4 sm:text-center sm:px-0\"\n  }, /*#__PURE__*/React.createElement(\"h3\", {\n    className: \"text-indigo-600 font-semibold\"\n  }, \"Pricing\"), /*#__PURE__*/React.createElement(\"p\", {\n    className: \"text-gray-800 text-3xl font-semibold sm:text-4xl\"\n  }, \"Pay as you grow\"), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"max-w-xl\"\n  }, /*#__PURE__*/React.createElement(\"p\", null, \"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam efficitur consequat nunc.\"))), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"mt-16 justify-center sm:flex\"\n  }, plans.map((item, idx) => /*#__PURE__*/React.createElement(\"div\", {\n    key: idx,\n    className: `relative flex-1 flex items-stretch flex-col mt-6 sm:mt-0 sm:rounded-xl sm:max-w-md ${item.isMostPop ? \"bg-white shadow-lg sm:border\" : \"\"}`\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"p-4 py-8 space-y-4 border-b md:p-8\"\n  }, /*#__PURE__*/React.createElement(\"span\", {\n    className: \"text-indigo-600 font-medium\"\n  }, item.name), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"text-gray-800 text-3xl font-semibold\"\n  }, \"$\", item.price, \" \", /*#__PURE__*/React.createElement(\"span\", {\n    className: \"text-xl text-gray-600 font-normal\"\n  }, \"/mo\")), /*#__PURE__*/React.createElement(\"p\", null, item.desc), /*#__PURE__*/React.createElement(\"button\", {\n    className: \"px-3 py-3 rounded-lg w-full font-semibold text-sm duration-150 text-white bg-indigo-600 hover:bg-indigo-500 active:bg-indigo-700\"\n  }, \"Get Started\")), /*#__PURE__*/React.createElement(\"ul\", {\n    className: \"p-4 py-8 space-y-3 md:p-8\"\n  }, /*#__PURE__*/React.createElement(\"li\", {\n    className: \"pb-2 text-gray-800 font-medium\"\n  }, /*#__PURE__*/React.createElement(\"p\", null, \"Features\")), item.features.map((featureItem, idx) => /*#__PURE__*/React.createElement(\"li\", {\n    key: idx,\n    className: \"flex items-center gap-5\"\n  }, /*#__PURE__*/React.createElement(\"svg\", {\n    xmlns: \"http://www.w3.org/2000/svg\",\n    className: \"h-5 w-5 text-indigo-600\",\n    viewBox: \"0 0 20 20\",\n    fill: \"currentColor\"\n  }, /*#__PURE__*/React.createElement(\"path\", {\n    \"fill-rule\": \"evenodd\",\n    d: \"M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z\",\n    \"clip-rule\": \"evenodd\"\n  })), featureItem))))))));\n}\n\n;"}
rtl: {"preview":"function App() {\n  const plans = [{\n    name: \"شركة ناشئة\",\n    desc: \"العميل مهم جدا، العميل سيتبعه.\",\n    price: 12,\n    isMostPop: false,\n    features: [\"هناك حقيقة مثبتة\", \"هو ببساطة نص شكلي\", \"لوريم إيبسوم ليس نصاَ عشوائياً\", \"عاد لينتشر مرة أخرى\", \"لكن الغالبية تم تعديلها\", \"عام في القدم\", \" ليس هناك أي كلمات أو عبارات\"]\n  }, {\n    name: \"مَشرُوع\",\n    desc: \"العميل مهم جدا، العميل سيتبعه.\",\n    price: 32,\n    isMostPop: true,\n    features: [\"هناك حقيقة مثبتة\", \"هو ببساطة نص شكلي\", \"لوريم إيبسوم ليس نصاَ عشوائياً\", \"عاد لينتشر مرة أخرى\", \"لكن الغالبية تم تعديلها\", \"عام في القدم\", \" ليس هناك أي كلمات أو عبارات\"]\n  }];\n  return /*#__PURE__*/React.createElement(\"section\", {\n    className: \"relative py-14\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"absolute top-0 w-full h-[473px]\",\n    style: {\n      background: \"linear-gradient(152.92deg, rgba(192, 132, 252, 0.2) 4.54%, rgba(232, 121, 249, 0.17) 34.2%, rgba(192, 132, 252, 0.1) 77.55%)\"\n    }\n  }), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"max-w-screen-xl mx-auto text-gray-600 sm:px-4 md:px-8\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"relative max-w-xl mx-auto space-y-3 px-4 sm:text-center sm:px-0\"\n  }, /*#__PURE__*/React.createElement(\"h3\", {\n    className: \"text-indigo-600 font-semibold\"\n  }, \"\\u0627\\u0644\\u062A\\u0633\\u0639\\u064A\\u0631\"), /*#__PURE__*/React.createElement(\"p\", {\n    className: \"text-gray-800 text-3xl font-semibold sm:text-4xl\"\n  }, \"\\u0627\\u062F\\u0641\\u0639 \\u0643\\u0645\\u0627 \\u062A\\u0646\\u0645\\u0648\"), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"max-w-xl\"\n  }, /*#__PURE__*/React.createElement(\"p\", null, \"\\u0627\\u0644\\u0639\\u0645\\u064A\\u0644 \\u0645\\u0647\\u0645 \\u062C\\u062F\\u0627\\u060C \\u0627\\u0644\\u0639\\u0645\\u064A\\u0644 \\u0633\\u064A\\u062A\\u0628\\u0639\\u0647. \\u0644\\u0627 \\u062A\\u0648\\u062C\\u062F \\u0646\\u062A\\u064A\\u062C\\u0629 \\u0627\\u0644\\u0622\\u0646.\"))), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"mt-16 justify-center sm:flex\"\n  }, plans.map((item, idx) => /*#__PURE__*/React.createElement(\"div\", {\n    key: idx,\n    className: `relative flex-1 flex items-stretch flex-col mt-6 sm:mt-0 sm:rounded-xl sm:max-w-md ${item.isMostPop ? \"bg-white shadow-lg sm:border\" : \"\"}`\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"p-4 py-8 space-y-4 border-b md:p-8\"\n  }, /*#__PURE__*/React.createElement(\"span\", {\n    className: \"text-indigo-600 font-medium\"\n  }, item.name), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"text-gray-800 text-3xl font-semibold\"\n  }, \"$\", item.price, \" \", /*#__PURE__*/React.createElement(\"span\", {\n    className: \"text-xl text-gray-600 font-normal\"\n  }, \"/\\u0634\\u0647\\u0631\")), /*#__PURE__*/React.createElement(\"p\", null, item.desc), /*#__PURE__*/React.createElement(\"button\", {\n    className: \"px-3 py-3 rounded-lg w-full font-semibold text-sm duration-150 text-white bg-indigo-600 hover:bg-indigo-500 active:bg-indigo-700\"\n  }, \"\\u062F\\u0639\\u0646\\u0627 \\u0646\\u0628\\u062F\\u0621\")), /*#__PURE__*/React.createElement(\"ul\", {\n    className: \"p-4 py-8 space-y-3 md:p-8\"\n  }, /*#__PURE__*/React.createElement(\"li\", {\n    className: \"pb-2 text-gray-800 font-medium\"\n  }, /*#__PURE__*/React.createElement(\"p\", null, \"\\u0627\\u0644\\u0645\\u0645\\u064A\\u0632\\u0627\\u062A\")), item.features.map((featureItem, idx) => /*#__PURE__*/React.createElement(\"li\", {\n    key: idx,\n    className: \"flex items-center gap-5\"\n  }, /*#__PURE__*/React.createElement(\"svg\", {\n    xmlns: \"http://www.w3.org/2000/svg\",\n    className: \"h-5 w-5 text-indigo-600\",\n    viewBox: \"0 0 20 20\",\n    fill: \"currentColor\"\n  }, /*#__PURE__*/React.createElement(\"path\", {\n    \"fill-rule\": \"evenodd\",\n    d: \"M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z\",\n    \"clip-rule\": \"evenodd\"\n  })), featureItem))))))));\n}","vue":{"vueTail":[],"vueCss":[]},"react":{"jsxTail":[{"label":"App.jsx","code":"export default () => {\n\n    const plans = [\n        {\n            name: \"شركة ناشئة\",\n            desc: \"العميل مهم جدا، العميل سيتبعه.\",\n            price: 12,\n            isMostPop: false,\n            features: [\n                \"هناك حقيقة مثبتة\",\n                \"هو ببساطة نص شكلي\",\n                \"لوريم إيبسوم ليس نصاَ عشوائياً\",\n                \"عاد لينتشر مرة أخرى\",\n                \"لكن الغالبية تم تعديلها\",\n                \"عام في القدم\",\n                \" ليس هناك أي كلمات أو عبارات\",\n            ],\n        },\n        {\n            name: \"مَشرُوع\",\n            desc: \"العميل مهم جدا، العميل سيتبعه.\",\n            price: 32,\n            isMostPop: true,\n            features: [\n                \"هناك حقيقة مثبتة\",\n                \"هو ببساطة نص شكلي\",\n                \"لوريم إيبسوم ليس نصاَ عشوائياً\",\n                \"عاد لينتشر مرة أخرى\",\n                \"لكن الغالبية تم تعديلها\",\n                \"عام في القدم\",\n                \" ليس هناك أي كلمات أو عبارات\",\n            ],\n        },\n    ];\n\n    return (\n        <section className='relative py-14'>\n            <div className=\"absolute top-0 w-full h-[473px]\" style={{ background: \"linear-gradient(152.92deg, rgba(192, 132, 252, 0.2) 4.54%, rgba(232, 121, 249, 0.17) 34.2%, rgba(192, 132, 252, 0.1) 77.55%)\" }}></div>\n            <div className=\"max-w-screen-xl mx-auto text-gray-600 sm:px-4 md:px-8\">\n                <div className='relative max-w-xl mx-auto space-y-3 px-4 sm:text-center sm:px-0'>\n                    <h3 className=\"text-indigo-600 font-semibold\">\n                        التسعير\n                    </h3>\n                    <p className='text-gray-800 text-3xl font-semibold sm:text-4xl'>\n                        ادفع كما تنمو\n                    </p>\n                    <div className='max-w-xl'>\n                        <p>\n                            العميل مهم جدا، العميل سيتبعه. لا توجد نتيجة الآن.\n                        </p>\n                    </div>\n                </div>\n                <div className='mt-16 justify-center sm:flex'>\n                    {\n                        plans.map((item, idx) => (\n                            <div key={idx} className={`relative flex-1 flex items-stretch flex-col mt-6 sm:mt-0 sm:rounded-xl sm:max-w-md ${item.isMostPop ? \"bg-white shadow-lg sm:border\" : \"\"}`}>\n                                <div className=\"p-4 py-8 space-y-4 border-b md:p-8\">\n                                    <span className='text-indigo-600 font-medium'>\n                                        {item.name}\n                                    </span>\n                                    <div className='text-gray-800 text-3xl font-semibold'>\n                                        ${item.price} <span className=\"text-xl text-gray-600 font-normal\">/شهر</span>\n                                    </div>\n                                    <p>\n                                        {item.desc}\n                                    </p>\n                                    <button className='px-3 py-3 rounded-lg w-full font-semibold text-sm duration-150 text-white bg-indigo-600 hover:bg-indigo-500 active:bg-indigo-700'>\n                                        دعنا نبدء\n                                    </button>\n                                </div>\n                                <ul className='p-4 py-8 space-y-3 md:p-8'>\n                                    <li className=\"pb-2 text-gray-800 font-medium\">\n                                        <p>المميزات</p>\n                                    </li>\n                                    {\n                                        item.features.map((featureItem, idx) => (\n                                            <li key={idx} className='flex items-center gap-5'>\n                                                <svg\n                                                    xmlns='http://www.w3.org/2000/svg'\n                                                    className='h-5 w-5 text-indigo-600'\n                                                    viewBox='0 0 20 20'\n                                                    fill='currentColor'>\n                                                    <path\n                                                        fill-rule='evenodd'\n                                                        d='M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z'\n                                                        clip-rule='evenodd'></path>\n                                                </svg>\n                                                {featureItem}\n                                            </li>\n                                        ))\n                                    }\n                                </ul>\n                            </div>\n                        ))\n                    }\n                </div>\n            </div>\n        </section>\n    )\n}"}],"jsxCss":[]}}
slug: /pricing-sections
id: 262463f9-d0df-4c9c-9e6e-ef544e8e316c
created_at: 1670763480676
---